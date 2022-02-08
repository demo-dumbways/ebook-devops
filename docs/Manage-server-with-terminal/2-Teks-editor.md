---
sidebar_position: 2
---

# 2. Teks Editor(Nano)
import useBaseUrl from '@docusaurus/useBaseUrl';

**Text Editor** adalah sebuah aplikasi yang berjalan di atas terminal, gunanya untuk melakukan manipulasi data pada sebuah file. Pada sebuah server kita wajib mengetahui penggunaan text editor karena di server tidak ada aplikasi yang bersifat GUI.

## Kenapa perlu belajar Teks editor ?
Karena kita sebagai seorang DevOps engineer pasti akan membuat suatu konfigurasi tertentu untuk memanage suatu aplikasi maupun server. Maka dari itu kita perlu mengetahui beberapa shortcut-shortcut yang dapat membantu kita.

## nano shortcut :
Secara default **nano** sudah terinstall pada sistem operasi linux, untuk memeriksanya kalian bisa gunakan perintah berikut :

```shell
nano --version
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/nano1.png')} height="400px"/>
</center>

### 1. Membuka nano
cara membuka file nano dapat menggunakan perintah berikut

```shell
nano (file-name)
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano2.png')} height="400px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano3.png')} height="400px"/>
</center>

```shell
nano (location/folder/file-name)
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano4.png')} height="400px"/>
</center>


<center>
<img alt="image1" src={useBaseUrl('img/docs/nano5.png')} height="400px"/>
</center>

keterangan : location/folder/README.MD merupakan file yang lokasinya berada dalam folder/directory. 

### 2. Exit From teks editor nano

`ctrl + X` untuk keluar dari editor. Jika melakukan perubahan maka akan dimintai konfirmasi apakah perubahan akan disimpan / tidak. Ketik **Y** untuk yes, dan **N** untuk No kemudian tekan **Enter**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano6.png')} height="400px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano7.png')} height="400px"/>
</center>

keterangan : jika kalian ingin mengubah nama dari file, kalian dapat mengubah nama dari yang sebelumnya **README.MD** menjadi **(nama yang kalian inginkan).

`ctrl + O` adalah untuk menyimpan perubahan file tanpa harus keluar dari **teks editor nano**. Kemudian tekan **Enter**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano8.png')} height="400px"/>
</center>

### 3. Search on nano
`ctrl + W` adalah untuk mencari teks. Masukkan value ke kolom pencarian kemudian tekan **Enter**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano9.png')} height="400px"/>
</center>

### 4. Choose teks
`ALT + A` : adalah untuk memilih teks, cukup arahkan cursor sesuai teks yang ingin di select.

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano10.png')} height="280px"/>
</center>

### 5. Copy and Paste on nano
`ALT + 6` : untuk melakukan copy teks yang sudah di select

`CTRL + U` : untuk melakukan paste teks yang sudah di copy

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano10.png')} height="280px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano11.png')} height="280px"/>
</center>

### 6. Cut teks and Paste on nano
`CTRL + K` : untuk melakukan cut pada text yang sudah di select

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano12.png')} height="400px"/>
</center>

`CTRL + U` : untuk melakukan paste teks yang sudah di cut

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano13.png')} height="400px"/>
</center>

### 7. Move cursor
`CTRL + A` : untuk pindah cursor ke awal baris

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano14.png')} height="400px"/>
</center>

`CTRL + E` : untuk pindah cursor ke akhir baris

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano15.png')} height="400px"/>
</center>

### 8. Take Contents from another file

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano16.png')} height="400px"/>
</center>

keterangan : kalau kita lihat disini saya memilik file bernama `index.html` di dalam directory `dumbways.id`. Sekarang kita akan coba untuk mengambil isi dari file `index.html` tersebut ke dalam file `README.MD` kita.

`CTRL + R` : untuk mengambil isi dari suatu file 

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano17.png')} height="400px"/>
</center>

keterangan : masukan lokasi yang sesuai dengan file yang isinya ingin kalian ambil

<center>
<img alt="image1" src={useBaseUrl('img/docs/nano18.png')} height="400px"/>
</center>