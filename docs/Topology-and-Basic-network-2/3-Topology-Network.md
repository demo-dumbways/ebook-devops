---
sidebar_position: 3
---

# 3. Topology Network 
import useBaseUrl from '@docusaurus/useBaseUrl';

**Topology** adalah metode atau cara yang digunakan agar bisa menghubungkan satu komputer dengan komputer lainnya. Struktur atau jaringan yang digunakan untuk menghubungkan satu komputer dengan komputer lainnya bisa dengan menggunakan kabel atau nirkabel.

## Jenis-Jenis Topology

### 1. Topology Mesh

<center> 
     <img alt="image1" src={useBaseUrl('img/docs/image-21.png')} height="200px"/>
</center>

   Topologi Mesh ini menerapkan hubungan antar sentral secara penuh. Jumlah saluran harus disediakan untuk membentuk jaringan mesh. **Topology Mesh** ini merupakan jaringan peer to peer.

 - **Karakteristik Mesh**
   - Tidak ada client server, semuanya dapat bertindak sebagai client dan server
   - Bentuk mesh yang sangat sederhana ialah array dua dimensi tempat masing-masing simpul juga saling terhubung dengan keempat tetangganya.

### 2. Topology Bus

<center>
     <img alt="image1" src={useBaseUrl('img/docs/image-22.png')} height="190px"/>
</center>

   Topologi ini dibangun dengan kabel coaxial yang dibentang kemudian beberapa komputer dihubungkan pada kabel tersebut. Kedua ujung jaringan harus diakhiri dengan sebuah terminator.

 - **Karakteristik Bus**
   - Setiap komputer dalam suatu jaringan terhubung melalui kabel tunggal sebagai media transmisi.
   - Kabel tunggal tersebut dapat berfungsi sebagai backbone yang menjadi jalur data.
   - Setiap ujung kabel utama terpasang terminator untuk bisa menghentikan sinyal dan mencegah terjadinya tabrakan sinyal

### 3. Topology Ring

<center>
    <img alt="image1" src={useBaseUrl('img/docs/image-23.png')} height="190px"/>
</center>

   Topologi ring semua workstation dan server dihubungkan sehingga terbentuk sebuah pola lingkaran. Tiap workstation atau server akan menerima dan melewatkan informasi dari satu komputer ke komputer lain.

- **Karakteristik Ring**
   - Setiap komputer atau perangkat yang terhubung secara langsung satu dengan yang lainnya dalam satu jaringan.
   - Dalam proses pengiriman data pada suatu waktu hanya bisa dilakukan oleh satu titik dengan proses pengiriman satu jalur.
   - Setiap paket data atau informasi bisa mengalir melalui kanan atau kiri titik sehingga hal ini dapat menghindari collision.
   - Kerusakan pada satu titik bisa mengakibatkan kerusakan pada titik-titik lainnya yang saling terhubung dalam satu jaringan.

### 4. Topology Star

<center>
    <img alt="image1" src={useBaseUrl('img/docs/image-24.png')} height="200px"/>
</center>

   Topologi star, masing-masing workstation dihubungkan secara langsung ke server. Sehingga jalur bandwidth akan semakin lebar dan meningkatkan kinerja jaringan secara keseluruhan.

- **Karakteristik Star**
   - Dari berbagai node dapat berkomunikasi secara langsung pada central node dengan trafik yang mengalir dari node central. 
   - Jaringan tidak mudah terganggu yang dapat disebabkan mengalami suatu kerusakan.
   - Topologi star dapat dengan mudah dikembangkan karena dari masing-masing node mempunyai kabel yang saling terhubung.

### 5. Topology Tree

<center>
    <img alt="image1" src={useBaseUrl('img/docs/image-25.png')} height="190px"/>
</center>

   Topologi ini merupakan gabungan dari beberapa topologi yang ada (star dan bus), yang bisa memadukan kinerja dari beberapa topologi.

- **Karakteristik Tree**
   - Proses pengiriman data dari klien pengirim ke klien penerima harus melalui hub (pusat kendali).
   - Pusat data dan kendali jaringan dipegang oleh sebuah hub sebagai kabel utama yang menghubungkan beberapa hub.
   - Terdapat kabel utama (backbone) yang berfungsi sebagai penghubung antar jaringan.
   - Mempunyai tingkatan dalam jaringan.