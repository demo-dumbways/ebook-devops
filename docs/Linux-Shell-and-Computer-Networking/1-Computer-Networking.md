---
sidebar_position: 1
---

# 1. Computer Networking

import useBaseUrl from '@docusaurus/useBaseUrl';

**Jaringan Komputer** adalah koneksi antara 2 komputer atau lebih, yang saling terhubung dengan media transmisi kabel atau tanpa kabel (wireless). Komputer saling terkoneksi apabila komputer tersebut bisa saling bertukar data / informasi, berbagi resource yang dimiliki seperti file, printer, hard disk, dll.

## Kenapa Harus Jaringan Komputer ?
Berikut adalah alasan kenapa harus mempelajari jaringan komputer:
- Mempercepat arus informasi 
- Mempermudah komunikasi antar individu 
- Mempercepat proses pengiriman data dan juga sumberdaya 
- Membantu mengkoneksikan kantor cabang yang berbeda pulau dan juga benua

## 1.1 Network Types
Jaringan komputer memiliki tipe-tipe sebagai berikut :

### 1. Jaringan client - server
**Server** adalah komputer yang menyediakan fasilitas bagi komputer-komputer lain di dalam suatu jaringan. **Client** adalah komputer-komputer yang menerima atau menggunakan fasilitas yang disediakan oleh server.

**Keunggulan Jaringan client - server**
- Kecepatan akses tinggi
- Keamanan dan backup data lebih baik

<center>
<img alt="image1" src={useBaseUrl('img/docs/net1.png')} height="200px"/>
</center>

**Kelemahan Jaringan client - server**
- Biaya operasional lebih mahal
- Diperlukan adanya satu komputer khusus untuk server
- Kelangsungan jaringan sangat bergantung pada server.

### 2. Jaringan peer - peer
Jaringan ini adalah **non-dedicated server**, karena server tidak berperan sebagai server murni melainkan sekaligus dapat berperan sebagai workstation. Artinya setiap workstation dapat bertindak sebagai **server** maupun **client**.

**Keunggulan peer - peer**
- Antar komputer dalam jaringan ini dapat berbagi fasilitas yang dimiliki
- Kelangsungan kerja jaringan tidak bergantung pada satu server.

<center>
<img alt="image1" src={useBaseUrl('img/docs/net2.png')} height="230px"/>
</center>

**Kelemahan Jaringan peer - peer**
- Sistem keamanan jaringan ditentukan oleh masing-masing user
- Data jaringan tersebar di masing-masing komputer , maka backup harus di lakukan oleh masing-masing komputer.

## 1.2 Jenis IP Address
**IP Address** adalah **Internet Protocol Address**, serangkaian angka unik milik perangkat yang terhubung ke jaringan yang lebih luas. IP Address diperlukan agar perangkat dan server dapat bertukar informasi satu sama lain.

### 1. IP Address Publik
IP Address Publik adalah alamat IP yang digunakan router untuk berkomunikasi dengan jaringan yang lebih luas. Diberikan oleh penyedia layanan internet (ISP), dimana terdapat informasi sehingga dapat dilacak.

### 2. IP Address Private :
IP Address Private adalah alamat IP pribadi yang dimiliki oleh setiap perangkat, entah itu laptop, smart TV atau smartphone yang terhubung ke jaringan lokal.

**Gambaran perbedaan IP Public dengan IP Private**

<center>
<img alt="image1" src={useBaseUrl('img/docs/net3.png')} height="350px"/>
</center>

## 1.3 Sifat-Sifat IP Address :

### 1. IP Address Dinamis
**IP Address Dinamis** merupakan pemberian IP secara otomatis dalam sebuah jaringan baik itu bersifat IP publik atau IP private. IP ini akan berubah-ubah setiap waktu.

### 2. IP Address Statis
**IP Address Statis** merupakan pemberian IP yang tidak akan berubah, harus di konfigurasi manual jika ingin menggunakan IP statis.

**Gambaran perbedaan dari sifat IP Dinamis sedangkan IP Statis**

<center>
<img alt="image1" src={useBaseUrl('img/docs/net4.png')} height="350px"/>
</center>

