---
sidebar_position: 4
---

# 4. Load Balancing

import useBaseUrl from '@docusaurus/useBaseUrl';

## 4.1 Apa itu Load Balancing?
**Load Balancing** adalah suatu jaringan komputer yang menggunakan metode untuk mendistribusikan beban kerjaan pada dua atau bahkan lebih suatu koneksi jaringan secara seimbang agar pekerjaan dapat berjalan optimal dan tidak overload (kelebihan) beban pada salah satu jalur koneksi.

## 4.2 Kenapa Harus Load Balancing?
Jika kita memiliki website atau aplikasi yang telah digunakan hingga ribuan, ratusan atau bahkan jutaan pengguna maka kita harus melakukan load balancing pada aplikasi tersebut agar tidak down, karena beban akses pengguna dibagi ke beberapa server sekaligus.

## 4.3 Membuat Konfigurasi Load Balancing
- Untuk membuat Load Balancing kalian harus membuat server baru lagi. Untuk cara membuat server kalian ikuti saja step by step seperti saat pertemuan Fundamental DevOps : [Install Ubuntu Server](/Fundamental-DevOps/5-Install-Ubuntu-Server.md)

- Jika server kalian sudah terbuat maka buatlah aplikasi sederhana sama seperti pertemuan sebelumnya (node.js). setelah itu jalankan aplikasi tersebut.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/b1.png')} height="500px"/>
  </center>

- Sekarang kita sudah mempunyai 2 buah server untuk aplikasi kita.
- Sekarang kita akan coba untuk membuat konfigurasi load balancing.
- Pertama-tama kita masuk ke dalam konfigurasi **reverse proxy** yang sudah kita buat sebelumnya.

```shell
sudo nano sudo nano /etc/nginx/dumbways/my.reverse-proxy.conf
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/b2.png')} height="500px"/>
  </center>

- Selanjutnya kita akan tambahkan konfigurasi ke dalam file `my.reverse-proxy.conf`. Sekarang kita akan coba tambahkan beberapa konfigurasi, kalian dapat menggunakan konfigurasi di bawah ini.

  ```shell
  upstream domain { 
      server 192.168.64.6:3000;
      server 192.168.64.2:3000;
  }
  server { 
      server_name mydomain.xyz; 
    
      location / { 
               proxy_pass http://domain;
      }
  }
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/b3.png')} height="500px"/>
  </center>


keterangan : 
- Pada bagian **upstream** kalian dapat mengganti nama **domain** dengan nama yang kalian inginkan. 
- Pada bagian **server** masukan **IP** dari server kalian, setelah itu diikuti dengan port aplikasi.
- Selanjutnya pada bagian **proxy_pass** ubah dari yang sebelumnya adalah alamat **IP** dari aplikasi kalian, sekarang kalian samakan dengan nama **upstream** yang ada di konfigurasi kalian.

- Jika sudah sekarang kita coba cek apakah konfigurasi yang sudah kita buat tadi itu error atau tidak.

  ```shell
  sudo nginx -t
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/b4.png')} height="500px"/>
  </center>

- Jika tidak ada error jalankan perintah `restart nginx` untuk merestart `nginx` kita, karena kita sudah menambahkan suatu konfigurasi baru di dalam file **reverse proxy** kita.

```shell
sudo systemctl restart nginx
```
  <center>
  <img alt="image1" src={useBaseUrl('img/docs/b5.png')} height="500px"/>
  </center>

- Selanjutnya jalankan aplikasi kita yang ada di server kita.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/b6.png')} height="500px"/>
  </center>


- Jika sudah sekarang coba buka web browser kalian setelah itu coba akses nama domain kalian.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web18.png')} height="500px"/>
  </center>

- Untuk make sure apakah load balancing yang sudah kita buat tadi berjalan dengan baik atau tidak, kita coba untuk mematikan satu aplikasi kita.
- Kita masuk ke dalam salah satu server aplikasi kita, setelah itu kalian hentikan aplikasi kalian `CTRL + C`.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/b7.png')} height="500px"/>
  </center>

- Sekarang kita coba akses web browser kita lagi setelah itu akses nama domain kalian.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web18.png')} height="500px"/>
  </center>

  :::info
  Jika aplikasi kalian masih bisa di akses berarti **konfigurasi Load Balance** kalian berhasil dan tidak ada error
  :::