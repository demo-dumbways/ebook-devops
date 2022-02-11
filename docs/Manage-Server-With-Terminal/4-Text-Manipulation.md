---
sidebar_position: 4
---

# 4. Teks Manipulation

import useBaseUrl from '@docusaurus/useBaseUrl';

Pada dasarnya kita bisa melakukan manipulasi pada **sebuah file** menggunakan terminal, tanpa menggunakan teks editor seperti **nano**.

## Berikut adalah contoh beberapa perintah yang dapat digunakan :

### 1. cat
`Cat` adalah salah satu perintah yang berfungsi untuk membuat daftar konten atau isi file pada standard output (sdout). Yang kalian tahu pasti perintah `cat` hanya bisa untuk melihat isi dari suatu file, sebenarnya tidak hanya itu.

Contoh penggunaan :

```shell
cat (file-name)
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks1.png')} height="500px"/>
</center>

keterangan : untuk melihat isi dari suatu file

```shell
cat > (file-name)
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks2.png')} height="500px"/>
</center>

keterangan : untuk membuat suatu file baru serta memasukkan teks, Jika sudah menambakan teks kalian dapat keluar dengan klik `CTRL + C`.

```shell
cat file1 file2 > file3
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks3.png')} height="500px"/>
</center>

keterangan : untuk menggabungkan dua buah file, dan menyimpannya ke dalam file3

### 2. sed
`Sed` adalah singkatan dari stream editor. Gunanya untuk memanipulasi teks dasar pada file. Dengan sed kita dapat mengganti teks dengan cepat. 

Contoh penggunaan :

```shell
sed -i 's/Hello/Holla/g' file3
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks4.png')} height="500px"/>
</center>

keterangan : mengganti semua kata **Hello** menjadi **Holla** pada file3 

### 3. grep
Grep merupakan perintah untuk melakukan pencarian sebuah text dalam sebuah file yang telah dibuat. 

Contoh penggunaan :

```shell
grep Dumbways file3
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks5.png')} height="500px"/>
</center>

keterangan : akan mencari kata **Dumbways** pada file3

```shell
grep -c Dumbways file3
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks6.png')} height="500px"/>
</center>

keterangan : akan menghitung jumlah kata “Dumbways” pada filetiga

```shell
grep Dumbways *
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks7.png')} height="500px"/>
</center>

keterangan : akan mencari semua file yang berisikan kata **Dumbways**

### 4. sort
`Sort` untuk mengurutkan data, baik itu secara ascending atau descending. 

Berikut adalah contoh penggunaan :

```shell
sort file4
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks8.png')} height="500px"/>
</center>

keterangan : untuk mengurutkan berdasarkan ascending

```shell
sort -r file4
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks9.png')} height="500px"/>
</center>

keterangan : untuk mengurutkan berdasarkan descending

### 5. echo
`Echo` digunakan untuk mencetak string / pesan dari hasil perintah lain. 

Berikut adalah contoh penggunaan

```shell
echo "Hello Dumbways!"
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks10.png')} height="500px"/>
</center>

keterangan : untuk mencetak string **

```shell
echo "Hello Dumbways!" >> file3
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/teks11.png')} height="500px"/>
</center>

keterangan : untuk mencetak kata **Hello Dumbways!** di file3

```shell
echo "Replace semua data" > file5
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/teks12.png')} height="500px"/>
</center>

keterangan : untuk mereplace semua data di file5 dan menggantinya dengan **"Replace semua data"**

