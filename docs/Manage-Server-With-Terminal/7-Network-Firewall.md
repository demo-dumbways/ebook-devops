---
sidebar_position: 7
---

# 7. Network Firewall

import useBaseUrl from '@docusaurus/useBaseUrl';

## Apa itu Network Firewall?

**Network Firewall** merupakan perintah yang dapat digunakan untuk mengamankan sebuah server. 

Tools yang dapat kita gunakan adalah :
- IPTables dan UFW

**IPTables** merupakan sebuah modul di linux yang memberikan dukungan langsung terhadap kernel untuk keamanan sistem serta beberapa keperluan jaringan. Iptables juga dapat digunakan untuk melakukan seleksi terhadap paket-paket yang datang baik itu output, input berdasarkan IP, port dan sebagainya.

**UFW (Uncomplicated Firewall)** adalah salah satu fitur frontend iptables pada linux untuk mengkonfigurasi sistem firewall.

## Kenapa perlu Firewall?

**Firewall** merupakan garis pertahanan pertama dalam menjaga keamanan jaringan komputer. **Firewall** menjadi bagian penting dari teknologi sistem keamanan. Selain itu, berbagai jenis firewall bekerja sama untuk menyediakan suatu payung sistem perlindungan lengkap. 

Risiko utama komputer atau jaringan yang tidak dilindungi oleh firewall adalah sebagai berikut:

- Tanpa firewall, komputer akan menerima setiap koneksi ke jaringan dari siapapun. Sehingga rentan terhadap kejahatan cyber. 

- Tanpa firewall dapat membuat perangkat komputer memiliki akses terbuka, yang memungkinkan siapa saja dapat memegang kendali atas komputer dan jaringan pribadi. Peretas dapat melakukan pencurian data pribadi atau menghapus data tersebut.

## Cara Menggunakan UFW
### 1. ufw installation
Untuk melakukan Instalasi kalian bisa menggunakan perintah dibawah ini.

```shell
sudo apt install ufw -y
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw1.png')} height="500px"/>
</center>

### 2. ufw deny incoming
```shell
sudo ufw default deny incoming 
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw2.png')} height="500px"/>
</center>

keterangan : memblokir semua akses yang masuk

### 3. ufw allow outgoing
```shell
sudo ufw default allow outgoing
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw3.png')} height="500px"/>
</center>

keterangan : membuka semua akses yang keluar

### 4. ufw app list
```shell
sudo ufw app list
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw4.png')} height="500px"/>
</center>

keterangan : untuk menampilkan aplikasi yang didukung oleh ufw pada server

### 5. ufw allow nginx
```shell
sudo ufw allow "Nginx Full"
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw5.png')} height="500px"/>
</center>

keterangan : untuk mengizinkan akses dari luar ke dalam untuk aplikasi nginx

### 6. ufw allow
```shell
sudo ufw allow 22
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw6.png')} height="500px"/>
</center>

keterangan : untuk membuka akses port 22

### 7. ufw allow /tcp
**TCP/IP** adalah standar komunikasi data yang digunakan oleh komunitas internet dalam proses tukar-menukar data dari satu komputer ke komputer lain di dalam jaringan Internet.

Contoh :
- Koneksi yang masih menggunakan http://

```shell
sudo ufw allow 22/tcp
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw7.png')} height="500px"/>
</center>

keterangan : membuka akses untuk port 22 dengan koneksi tcp

### 8. ufw allow /udp
**UDP** adalah kepanjangan dari User Datagram Protocol. Salah satu protocol yang menjadi lapisan transport **TCP/IP** sehingga mendukung atau memungkinkan terjadinya komunikasi yang tidak andal (unreliable), tanpa adanya koneksi antar host jaringan yang menggunakan TCP/IP. 

Contoh :
- Koneksi yang masih menggunakan https://

```shell
sudo ufw allow 22/udp
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw8.png')} height="500px"/>
</center>

keterangan : membuka akses untuk port 22 dengan koneksi udp

### 9. ufw deny
```shell
sudo ufw deny 80
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw9.png')} height="500px"/>
</center>

keterangan : memblokir semua akses ke port 80

### 10. ufw delete deny
```shell
sudo ufw delete deny 80
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw10.png')} height="500px"/>
</center>

keterangan : menghapus konfigurasi, harus sama dengan perintah yang ingin di hapus.

### 12. ufw active and verbose
```shell
sudo ufw enable
```

keterangan : untuk menghidupkan firewall

```shell 
sudo ufw verbose
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ufw11.png')} height="500px"/>
</center>

keterangan : untuk melihat koneksi apa saja yang ada