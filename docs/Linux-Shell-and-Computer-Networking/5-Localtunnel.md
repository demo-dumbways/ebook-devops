---
sidebar_position: 5
---

# 5. Localtunnel

import useBaseUrl from '@docusaurus/useBaseUrl';

## 5.1 Apa itu Localtunnel?
**Localtunnel** adalah sebuah tools yang memungkinkan kita untuk berbagi layanan website dari lokal komputer ke publik dengan url akses yang disediakan oleh localtunnel.

**Ilustrasi bagaimana cara Localtunnel bekerja**

<center>
<img alt="image1" src={useBaseUrl('img/docs/localtunnel.png')} height="300px"/>
</center>

## 5.2 Kenapa Localtunnel ?
- Kita dapat membuat aplikasi web dapat diakses secara publik.
- Tidak perlu meletakkan web tersebut ke server online.
- Tidak perlu membeli domain.

## 5.3 Bagaimana Menggunakan Localtunnel?

Kita akan mencoba untuk menjalankan localtunnel agar server local kita dapat di akses secara publik. Berikut adalah step by step cara menggunakannya:

- Pertama-tama yang kita lakukan adalah instalalsi `node.js` menggunakan `nvm` untuk melakukan instalasi kalian dapat mengikuti langkah-langkah dibawah ini.
  
  ```shell
  sudo apt install curl
  ```
  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tun1.png')} height="400px"/>
  </center>

  ```shell
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tun2.png')} height="400px"/>
  </center>

  ```shell
  exec bash
  ```

  ```shell
  nvm install 14
  ```

  ```shell
  node -v
  ```

  ```shell
  npm -v
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tun3.png')} height="400px"/>
  </center>

- Selanjutnya kita akan melakukan instalasi `localtunnel` menggunakan `npm` yang sudah kita install.

  ```shell
  npm install -g localtunnel
  ```
  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tun4.png')} height="400px"/>
  </center>

- Sekarang kita akan melakukan instalasi `Nginx` yang sama seperti pertemuan sebelumnya.

  ```shell
  sudo apt install nginx
  ```

    Lalu nanti akan muncul notifikasi **Do you want to continue? [Y/n]** kalian ketik saja **Y**. Jika sudah maka instalasi akan berjalan.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s1.png')} height="400px"/>
  </center>

- Jika instalasi kalian telah selesai melakukan instalasi `Nginx`, Selanjutnya kita coba untuk mengakses nginx di web browser kita untuk mengecek apakah `Nginx` kita sudah berjalan atau belum.

- Coba kalian akses di web browser kalian, lalu masukkan IP dari server kalian.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tune1.png')} height="400px"/>
  </center>

- Sekarang kita coba untuk menggunakan localtunel untuk aplikasi `Nginx` yang sudah kita install.
- Untuk menjalankan localtunel kalian dapat mengikuti perintah di bawah ini.

  ```shell
  lt --port 80
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tune2.png')} height="400px"/>
  </center>

  keterangan : pastikan dibagian port telah sesuai dengan aplikasi kalian. Karena setiap aplikasi pasti mempunyai port yang berbeda-beda, kita ambil contoh saja dari aplikasi `node.js`, aplikasi node.js biasanya berjalan di atas port 3000.

- Jika sudah copy url yang ada di terminal kalian.
- Setelah itu coba kalian akses menggunakan Web.browser kalian.
  
  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tune3.png')} height="400px"/>
  </center>

- Jika sudah klik tombol `Click to Continue`.
- Selanjutnya kalian akan di arahkan ke aplikasi kalian. Dan aplikasi kalian sekarang sudah dapat di akses oleh public.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tune4.png')} height="400px"/>
  </center>