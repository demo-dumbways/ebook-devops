---
sidebar_position: 1
---

# 1. Web Server

import useBaseUrl from '@docusaurus/useBaseUrl';

## 1.1 Apa itu Web Server?
**Web Server** adalah sebuah software yang memberikan layanan berupa data. Berfungsi untuk menerima permintaan **HTTP** atau **HTTPS** dari client atau di kenal dengan **web browser (chrome atau firefox)**. Kemudian web server akan mengirimkan respon atas permintaan tersebut dalam bentuk halaman web.

## 1.2 Kenapa Harus Belajar Web Server?
Karena **Web server** memiliki peran penting dalam mengendalikan proses kerja dari sebuah website. Tanpa adanya web server, kamu tidak bisa melakukan permintaan data apapun pada suatu halaman atau page di web browser. 

## 1.3 Bagaimana Cara Kerja Web Server?

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web1.png')} height="400px"/>
  </center>

Pada ilustrasi di atas, dapat dilihat bahwa komputer client sedang melakukan request data yang berada pada server database melalui sebuah web server kemudian web server akan mengembalikan data tersebut dalam bentuk halaman website pada komputer client.

## 1.4 Fungsi Web Server
- Menyediakan data berdasarkan request atau permintaan yang masuk agar dapat menjamin keamanan sistem yang berjalan dengan lancar.
- Melakukan pemeriksaan terhadap sistem security yang berasal dari permintaan HTTP berdasarkan request client atau web browser.

## 1.5 Jenis-Jenis Web Server
- Apache
- Nginx
- Litespeed
- Lightpd

## 1.6 Instalasi Nginx dan Service Management
Sekarang kita akan mencoba untuk melakukan instalasi salah satu web server yang terkenal yaitu adalah **Nginx**.

Berikut adalah cara untuk melakukan Instalasi **Nginx**

```shell
sudo apt update; sudo apt upgrade
```

```shell
sudo apt install nginx
```

Lalu nanti akan muncul notifikasi **Do you want to continue? [Y/n]** kalian ketik saja **Y**. Jika sudah maka instalasi akan berjalan.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s1.png')} height="400px"/>
  </center>

Jika kalian sudah menjalankan beberapa perintah diatas kalian sudah berhasil untuk melakukan installasi **Nginx**. Kalian bisa check menggunakan perintah di bawah ini.

```shell
nginx -v
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web2.png')} height="400px"/>
  </center>

### 1. Nginx Status
```shell
sudo systemctl status nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s2.png')} height="400px"/>
  </center>


keterangan : perintah untuk melihat status dari `Nginx`.

### 2. Enable nginx
```shell
sudo systemctl enable nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s3.png')} height="400px"/>
  </center>


Keterangan : perintah untuk menghidupkan sistem dari `Nginx`

### 3. Start nginx
```shell
sudo systemctl start nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s4.png')} height="400px"/>
  </center>


keterangan : perintah untuk menjalankan sistem dari `Nginx`

### 4. Restart nginx
```shell
sudo systemctl restart nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s5.png')} height="400px"/>
  </center>


keterangan : perintah untuk merestart sistem dari `Nginx`

### 5. Reload nginx
```shell
sudo systemctl reload nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s6.png')} height="400px"/>
  </center>


keterangan : perintah untuk me-reload sistem dari `Nginx`

### 6. Disable nginx
```shell
sudo systemctl disable nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s7.png')} height="400px"/>
  </center>


keterangan : perintah untuk mematikan sistem dari `Nginx`

### 7. Stop nginx
```shell
sudo systemctl stop nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s8.png')} height="400px"/>
  </center>


keterangan : perintah untuk menghentikan sistem dari `Nginx`

### 8. Check Nginx
Kemudian untuk melihat nginx telah terinstall. Kalian dapat mengakses IP dari server kalian, maka akan terlihat seperti berikut, sebelum itu lakukan beberapa perintah berikut karena di tahapan sebelumnya kita telah menghentikan **Nginx** yang sudah kita install.

```shell
sudo systemctl enable nginx
```

```shell
sudo systemctl start nginx
```

```shell
sudo systemctl status nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web3.png')} height="400px"/>
  </center>

Jika sudah Kalian dapat mengakses IP dari server kalian, maka akan terlihat seperti berikut:

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/web4.png')} height="400px"/>
  </center>

