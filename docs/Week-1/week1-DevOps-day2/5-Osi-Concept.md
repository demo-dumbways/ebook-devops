---
sidebar_position: 5
---

# 5. OSI Concept
import useBaseUrl from '@docusaurus/useBaseUrl';

OSI adalah **Open System Interconnection**, yaitu model referensi yang diciptakan dari sebuah kerangka yang bersifat konseptual. Namun, saat ini telah berkembang dan menjadi sebuah standarisasi khusus berkaitan dengan koneksi komputer. 

**1. Physical Layer (Lapisan ke 1)**    : Layer physical pada OSI adalah lapisan yang berfungsi sebagai transmisi terhadap bit data.

**2. Data-Link Layer (Lapisan ke 2)**   : Data link layer bertugas untuk memeriksa bila terjadi kesalahan dalam menyalurkan transmisi terhadap bit data.

**3. Network Layer (Lapisan ke 3)**     : Network Layer bertugas untuk mendefinisikan alamat IP sehingga setiap komputer dapat saling terkoneksi dalam satu jaringan. Fungsi lainnya adalah melaksanakan proses routing dan membuat header untuk setiap paket data yang ada.

**4. Transport Layer (Lapisan ke 4)**   : Transport Layer bertugas untuk Melakukan transmisi data mulai dari session sampai ke network layer, Melakukan looping terhadap proses transmisi yang ada dalam paket data yang hilang. Dengan layer ini, data bisa disalurkan dari server menuju ke pengguna tanpa adanya gangguan.  

**5. Session Layer (Lapisan ke 5)**     : Layer session memiliki fungsi untuk mengendalikan dialog maupun melakukan pengelolaan terhadap koneksi suatu komputer. Bahkan layer ini juga bisa melakukan pemutusan koneksi internet pada suatu komputer.

**6. Presentation Layer (Lapisan ke 6)**: Lapisan Presentation berfungsi untuk mengidentifikasi sintaks yang dipakai suatu host jaringan untuk berkomunikasi.

**7. Application Layer (Lapisan ke 7)** : Application layer pada OSI adalah pusat terjadinya suatu interaksi antara user dengan aplikasi yang bekerja menggunakan fungsionalitas sebuah jaringan.

<img alt="image1" src={useBaseUrl('img/docs/image-28.png')} height="350px"/>

