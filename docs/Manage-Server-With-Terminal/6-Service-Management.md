---
sidebar_position: 6
---

# 6. Service Management
import useBaseUrl from '@docusaurus/useBaseUrl';

## 6.1 Apa itu Service Management?
**Systemd** adalah standar manager sistem linux saat ini. Fungsinya memberikan sebuah metode untuk mengaktifkan system resources, daemons dan proses lainnya baik itu ketika booting maupun ketika sistem berjalan.

Command yang digunakan untuk systemd adalah `systemctl`.

## 6.2 Kenapa Service Management ?
Kita harus mempelajari service management agar:
- Dapat menjalan aplikasi secara background.
- Dapat menjadikan aplikasi auto running ketika server di restart.

## 6.3 Macam-macam perintah dari Systemd
- Start	: Menjalankan service
- Restart	: Merestart service yang sedang berjalan
- Enable	: Mengaktifkan service ketika boot
- Disable	: Menonaktifkan service ketika boot
- Status	: Menampilkan status service

## 6.4 Contoh penggunaan Service Management
### 1. Nginx Instalation
```shell
sudo apt install nginx
```
  Lalu nanti akan muncul notifikasi **Do you want to continue? [Y/n]** kalian ketik saja **Y**. Jika sudah maka instalasi akan berjalan.

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s1.png')} height="500px"/>
  </center>

### 2. Nginx Status
```shell
sudo systemctl status nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s2.png')} height="500px"/>
  </center>


keterangan : perintah untuk melihat status dari `Nginx`.

### 3. Enable nginx
```shell
sudo systemctl enable nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s3.png')} height="500px"/>
  </center>


Keterangan : perintah untuk menghidupkan sistem dari `Nginx`

### 4. Start nginx
```shell
sudo systemctl start nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s4.png')} height="500px"/>
  </center>


keterangan : perintah untuk menjalankan sistem dari `Nginx`

### 5. Restart nginx
```shell
sudo systemctl restart nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s5.png')} height="500px"/>
  </center>


keterangan : perintah untuk merestart sistem dari `Nginx`

### 6. Reload nginx
```shell
sudo systemctl reload nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s6.png')} height="500px"/>
  </center>


keterangan : perintah untuk me-reload sistem dari `Nginx`

### 7. Disable nginx
```shell
sudo systemctl disable nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s7.png')} height="500px"/>
  </center>


keterangan : perintah untuk mematikan sistem dari `Nginx`

### 8. Stop nginx
```shell
sudo systemctl stop nginx
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/s8.png')} height="500px"/>
  </center>


keterangan : perintah untuk menghentikan sistem dari `Nginx`