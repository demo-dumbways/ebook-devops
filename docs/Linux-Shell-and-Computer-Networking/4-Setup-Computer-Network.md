---
sidebar_position: 4
---

# 4. Setup Computer Network

import useBaseUrl from '@docusaurus/useBaseUrl';

## 4.1 Apa itu Setup Computer Network?

Setup Computer Network merupakan cara seorang DevOps ataupun System Administrator untuk mengganti default IP pada sebuah server.

## 4.2 Kenapa Harus Setup Computer Network?

Pada dasarnya, IP pada sistem operasi server dapat berubah jika router atau internet yang digunakan berubah. Maka dari itu seorang DevOps juga perlu mempelajari bagaimana cara mengganti IP server dengan cara manual.

## 4.3 Bagaimana Setup Computer Network?

Jika kalian ingin melakukan perubahan untuk **IP** dari server yang sudah kalian buat kalian bisa gunakan perintah berikut

```shell
sudo nano /etc/netplan/00-installer-config.yaml
```

Jika kalian sudah menggunakan perintah di atas maka akan muncul text editor seperti gambar dibawah ini. Selanjut di bagian **addresses** kalian bisa ubah dengan IP yang kalian inginkan. Lalu untuk keluar dari teks editor ini kalian bisa menggunakan **ctrl + x** lalu **Y** setelah itu **Enter**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/custom1.png')} height="500px"/>
</center>

Selanjutnya untuk mengkonfirmasi customisasi **IP** yang sudah kalian buat tadi kalian bisa menggunakan perintah dibawah.

```shell
sudo netplan apply
```

Jika sudah maka kita coba cek apakah sudah terhubung dengan internet atau tidak bisa menggunakan perintah dibawah.

```shell
ping google.com
```

Jika sudah terhubung dengan internet maka akan muncul notifikasi seperti gambar di bawah ini.

<center>
<img alt="image1" src={useBaseUrl('img/docs/custom2.png')} height="500px"/>
</center>

Setelah itu kita dapat melakukan pengecekan terhadap IP yang telah diubah tersebut melalui remote server. Untuk me-remote server kalian bisa gunakan perintah seperti ini

```shell
ssh alvin@192.168.1.6
```
Pastikan dibagian user(alvin), dan IP(192.168.1.6) ubah dengan user dan IP server yang sudah kalian buat sebelumnya. Jika sudah nanti akan muncul **Are you sure you want to continue connecting** langsung ketik saja **yes**. Jika sudah masukkan Password dari Server yang sudah kalian buat sebelumnya.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm29.png')} height="300px"/>
</center>

Selanjutnya tahapan pertama yang harus kita lakukan pada saat sedang berada di dalam server yaitu melakukan update serta upgrade terlebih dahulu gunanya untuk menjaga agar system kita tetap up-to-date.

Untuk melakukan update dan upgrade, kalian bisa menggunakan perintah di bawah ini.

```shell
sudo apt update; sudo apt upgrade
```

Selanjutnya kita akan coba untuk menginstall aplikasi **Nginx**.
  
Kalian bisa gunakan perintah di bawah ini.  
```shell
sudo apt install nginx
```

Lalu nanti akan muncul notifikasi **Do you want to continue? [Y/n]** kalian ketik saja **Y**. Jika sudah maka instalasi akan berjalan.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm30.png')} height="350px"/>
</center>

Jika instalasi sudah selesai kita bisa cek dengan menggunakan perintah dibawah ini.

```shell
sudo systemctl status nginx
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm31.png')} height="350px"/>
</center>

Sekarang coba buka browser kalian, lalu masukkan **IP dari server kalian**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm32.png')} height="350px"/>
</center>