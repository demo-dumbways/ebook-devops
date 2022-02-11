---
sidebar_position: 3
---

# 3. Reverse Proxy

import useBaseUrl from '@docusaurus/useBaseUrl';

## 3.1 Apa itu Reverse Proxy?

**Reverse proxy** adalah konfigurasi standar yang digunakan untuk mengubah jalur traffic, misalkan aplikasi menggunakan port 3000 tetapi agar dapat di akses melalui port 80 maka harus menggunakan reverse proxy.

Berikut adalah konfigurasi dari **revese proxy**.

```shell
server { 
    server_name domain.com; 
    
    location / { 
             proxy_pass http://127.0.0.1:3000;
    }
}
```

## 3.2 Kenapa Harus Reverse Proxy?
Untuk mengamankan aplikasi yang berjalan pada server maka kita perlu untuk melakukan reverse proxy, supaya pengguna tidak dapat mengakses aplikasi kita secara langsung.

## 3.3 Membuat Konfigurasi Revese Proxy
Untuk membuat reverse proxy dapat mengikuti langkah-langkah berikut :

- Pertama-tama masuk ke folder nginx setelah itu buat suatu directory baru telebih dahulu.

  ```shell
  cd /etc/nginx
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web5.png')} height="400px"/>
  </center>

  ```shell
  sudo mkdir dumbways
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web6.png')} height="400px"/>
  </center>

- Setelah itu masuk ke **directory** yang sudah kalian buat, setelah itu buat suatu file dengan nama `my.reverse-proxy.conf`

  ```shell
  cd dumbways
  ```

  ```shell
  sudo nano my.reverse-proxy.conf
  ```


  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web7.png')} height="400px"/>
  </center>

- Setelah itu masukkan konfigurasi berikut:

  ```shell
  server { 
      server_name mydomain.xyz; 
    
      location / { 
               proxy_pass http://127.0.0.1:3000;
      }
  }
  ```

  :::info
  pastikan IP dan port 3000 di ganti sesuai aplikasi yang digunakan.
  :::

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web8.png')} height="400px"/>
  </center>

- Jika sudah simpan konfigurasi yang sudah kalian buat tadi.
- Selanjutnya keluar dari directory `dumbways`, setelah itu masuk ke dalam file `nginx.conf`.

  ```shell
  cd ..
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web9.png')} height="400px"/>
  </center>

  ```shell
  sudo nano nginx.conf
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web10.png')} height="400px"/>
  </center>


- Selanjutnya pergi ke-bagian **include**, setelah itu masukan lokasi dari directory yang bersi konfigutasi yang sudah kalian buat tadi.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web11.png')} height="400px"/>
  </center>

  :::info
  `/*;` menandakan file `nginx.conf` akan membaca seluruh file yang berada di dalam directory **dumbways**
  :::

- Beberapa proses tadi adalah cara untuk membuat **reverse proxy** untuk aplikasi kita, kemudian pastikan untuk melakukan pengecekan konfigurasi dengan menjalankan perintah :

  ```shell
  sudo nginx -t
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web12.png')} height="400px"/>
  </center>

- Jika sudah sekarang kita tinggal melakukan `restart/reload` Nginx kita.

  ```shell
  sudo systemctl restart nginx
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web13.png')} height="400px"/>
  </center>

- Sekarang kita akan membuat sebuah virtual host. Untuk membuat virtual host kita harus masuk ke local server kita setelah itu masuk ke dalam file `/etc/hosts`.

  ```shel
  sudo nano /etc/hosts
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web14.png')} height="400px"/>
  </center>

- Setelah itu masukkan IP server kita selanjutnya masukkan nama domain yang kalian inginkan.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web15.png')} height="400px"/>
  </center>

- Jika sudah sekarang coba buka web.browser kalian setelah itu coba akses nama domain kalian.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web16.png')} height="400px"/>
  </center>

- Jika kita lihat disini adalah kita mendapatkan **502 Bad Gateway** kenapa?, karena kita belum menjalankan aplikasi kita. Sekarang kita coba untuk menjalankan aplikasi **dumbflix** yang sudah pernah kita pakai sebelumnya. Untuk menjalankan aplikasi `dumbflix` kalian dapat mengikuti langkah-langkah berikut ini.

  ```shell
  git clone https://github.com/dumbwaysdev/dumbflix-frontend.git
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/r1.png')} height="400px"/>
  </center>

  ```shell
  cd dumbflix-frontend
  ```

  ```shell
  npm install
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/r2.png')} height="400px"/>
  </center>

  keterangan : perintah di atas ini bertujuan untuk meng-install module dari aplikasi `node.js`

  ```shell
  npm start
  ```
  <center>
  <img alt="image1" src={useBaseUrl('img/docs/r3.png')} height="400px"/>
  </center>

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/r4.png')} height="400px"/>
  </center>

  keterangan : perintah di atas ini untuk menjalankan aplikasi

- Selanjutnya kita coba untuk me-refresh web.browser kita.
- Sekarang bisa kita lihat bahwa aplikasi kita sudah berjalan, dan dapat di akses oleh domain virtual yang kita buat.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/r5.png')} height="400px"/>
  </center>