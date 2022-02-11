---
sidebar_position: 3
---

# 3. Linux Shell
import useBaseUrl from '@docusaurus/useBaseUrl';

## 3.1 Apa itu Shell Linux?
**Shell Linux** merupakan program berbasis unix atau linux yang menghubungkan antara users dengan sistem operasi. **Shell script** yang biasa digunakan pada linux adalah **BASH (Bourne-Again-Shell).

## 3.2 Kenapa Harus Linux Shell?

Pada sistem operasi server berbasis unix/linux memiliki tampailan berbasis text, tidak seperti sistem operasi windows yang memiliki interface yang dapat di klik-klik. Sehingga memerlukan keahlian khusus untuk memanajemen server-server linux.

## 3.3 Perintah Dasar Linux:

### 1. sudo 
**sudo** adalah suatu perintah untuk memungkin kalian untuk menjalankan program sebagai pengguna lain.

Contoh penggunaanya adalah **sudo apt update; sudo apt upgrade** berfungsi untuk meng-update serta meng-upgrade sistem kita agar tetap up to date.

```shell
sudo apt update; sudo apt upgrade
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell1.png')} height="400px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell2.png')} height="400px"/>
</center>

### 2. mkdir 
**mkdir** adalah perintah untuk membuat suatu directory. Sebagai contoh coba kalian buat directory dengan nama **dumbways** seperti contoh dibawah ini.

```shell
mkdir dumbways
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell+.png')} height="400px"/>
</center>

### 3. ls 
**ls** adalah perintah untuk melihat list apa saja yang ada di directory.

```shell
ls
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell3.png')} height="400px"/>
</center>

### 4. ls -la 
**ls -la** adalah perintah untuk melihat semua list file dan directory yang ada serta menampilkan semua file maupun directory yang tersembunyi.

```shell
ls -la
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell4.png')} height="400px"/>
</center>

### 5. cd
**cd** adalah perintah untuk masuk ke dalam directory.

```shell
cd
``` 
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell5.png')} height="400px"/>
</center>

### 6. cd ..
**cd ..** adalah perintah untuk keluar dari directory.

```shell
cd ..
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell6.png')} height="400px"/>
</center>

### 7. touch
**touch** adalah perintah untuk membuat suatu file. Sebagai contoh coba kalian buat suatu file dengan nama **index.html**.

```shell
touch index.html
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell7.png')} height="400px"/>
</center>

### 8. cp
**cp** adalah perintah untuk meng-copy file serta mengubahnya dengan nama yang kalian inginkan. sebagai contoh coba kalian copy file **index.html** yang sudah kalian buat tadi lalu ubah dengan nama file **index**.

```shell
cp index.html index
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell8.png')} height="400px"/>
</center>

### 9. mv
**mv** adalah sebuah perintah untuk me-rename nama file, tetapi juga dapat digunakan untuk memindahkan suatu file ke directory tertentu. Sebagai contoh coba kalian ubah nama file **index** tadi dengan nama **index.js** lalu buat sebuah directory baru lalu pindahkan file **index.js** tadi ke directory yang sudah kalian buat.

```shell
mv index index.js
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell9.png')} height="400px"/>
</center>

```shell
mkdir studycase
```

```shell
mv index.js studycase
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell10.png')} height="400px"/>
</center>

### 10. echo 
**echo** adalah suatu perintah untuk menampilkan suatu string atau menyisipkan teks ke dalam file. Sebagai contoh coba kalian buatlah teks **hello dumbways** lalu sisipkan teks tersebut ke dalam file index.js.

```shell
echo "hello dumbways" > index.js
```

Sekarang coba kalian buat lagi teks **hello dumbways** tetapi buatlah di suatu file baru.

```shell
echo "hello dumbways" >> index
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell11.png')} height="400px"/>
</center>

### 11. cat
**cat** adalah suatu perintah untuk melihat isi dari suatu file. Sekarang coba implementasikan perintah **cat** untuk melihat isi dari suatu file yang sudah kalian buat sebelumnya.

```shell
cat index
```

```shell
cat index.js
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell12.png')} height="400px"/>
</center>

### 12. find
**find -type** adalah perintah untuk mencari suatu **file** maupun **directory**. Contoh disini kita akan mencari file index.js dan directory studycase yang sudah kita buat(**f** mengartikan file, sedangkan **d** adalah directory ).

```shell
find -type f -name index.js
```

```shell
find -type d -name studycase
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell13.png')} height="400px"/>
</center>

### 13. grep 
**grep** adalah suatu perintah untuk mencari teks di seluruh file. Sekarang kita coba untuk mencari teks yang sudah kita buat sebelumnya, kita juga akan mencoba mencari teks tetapi kita tidak tahu dimana lokasi file itu berada.

```shell
grep hello index.js
```

```shell
grep -r hello
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell14.png')} height="400px"/>
</center>

### 14. chmod
**chmod 777** adalah perintah untuk mengganti permission file maupun directory. Sekarang kita coba untuk mengganti permission untuk file **index.html** yang sudah kita buat sebelumnya.

```shell
sudo chmod 777 index.html
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/chmod777.png')} height="400px"/>
</center>

### 15. chown
**chown** adalah perintah untuk mengganti kepemilikan sebuah directory maupun file. Kita coba ganti kepemilikan file **index.html** tadi, dari yang sebelumnya adalah **user** kita sekarang kita ganti kepemilikannya menjadi **root**.

```shell
sudo chown root:root index.html
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell15.png')} height="400px"/>
</center>

### 16. history
**history** adalah perintah untuk melihat riwayat perintah yang sudah kita gunakan sebelumnya. 

```shell
history
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell16.png')} height="400px"/>
</center>

perintah **grep** juga bisa kita kombinasikan dengan history apabila, kita kesulitan untuk mencari riwayat perintah yang sudah kita jalankan. Kita cova implementasikan dengan mencari perintah **cat** di history kita.

```shell
history | grep cat
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell17.png')} height="400px"/>
</center>

### 17. ping
**ping** adalah perintah untuk memeriksa koneksi internet.

```shell
ping google.com
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell18.png')} height="400px"/>
</center>

### 18. wget 
**wget** adalah perintah untuk mendownload suatu file. Sekarang akan kita coba implementasikan perintah **wget** dengan mendownload file Wordpress, kalian bisa menggunakan url berikut: https://wordpress.org/latest.zip

```shell
wget https://wordpress.org/latest.zip
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell19.png')} height="400px"/>
</center>

### 19. unzip
**unzip** adalah perintah untuk **meng-extract zip file**. Untuk installasi unzip bisa menggunakan perintah dibawah ini.

```shell
sudo apt install unzip
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell20.png')} height="400px"/>
</center>

Sekarang kita coba extact **file zip** yang sebelumnya sudah kita download.

```shell
unzip latest.zip
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell21.png')} height="400px"/>
</center>

### 20. zip
**zip** adalah perintah untuk mengarsipkan/mengkompress suatu file atau directory. Untuk installasi zip bisa menggunakan perintah dibawah ini.

```shell
sudo apt install zip
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell22.png')} height="400px"/>
</center>

Sekarang kita coba implementasikan perintah zip untuk mengarsipkan/mengkompress directory **wordpress** yang sudah kita download sebelumnya lalu kita ubah nama untuk hasil kompressnya dengan nama **wordpress.zip**

```shell
zip -r wordpress.zip wordpress
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell23.png')} height="400px"/>
</center>

Hasil kompress :

<center>
<img alt="image1" src={useBaseUrl('img/docs/tambahan.png')} height="400px"/>
</center>

### 21. adduser
**adduser** adalah suatu perintah untuk membuat user baru untuk sistem.

```shell
sudo adduser alvin
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell24.png')} height="400px"/>
</center>

### 22. usermod
**usermod** adalah perintah untuk menambahkan **grup sudo** untuk **user** yang sudah kita buat, agar user dapat menggunakan perintah **sudo**.

```shell
sudo usermod -aG sudo alvin
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell25.png')} height="400px"/>
</center>

### 23. sudo su 
**sudo su** adalah perintah agar dapat masuk kedalam sistem root.

```shell
sudo su
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell26.png')} height="400px"/>
</center>

Untuk keluar dari root kalian bisa ketikan saja perintah seperti di bawah ini

```shell
exit
```
**sudo su** juga dapat digunakan untuk berpindah ke lain user. Contoh seperti di bawah ini kita masuk ke dalam user yang sudah kita buat sebelumya.

```shell 
sudo su alvin
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell27.png')} height="400px"/>
</center>

### 24. rm
**rm** adalah perintah untuk menghapus suatu file. Contoh disini coba buat satu buah file baru setelah itu kita akan menghapus file tersebut. 

```shell
rm file1
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell28.png')} height="400px"/>
</center>

**rmdir** adalah perintah untuk menghapus suatu directory. Contoh disini kita coba membuat satu directory baru lalu kita coba untuk menghapus directory yang sudah kita buat tadi.

```shell
rmdir devops
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/shell29.png')} height="400px"/>
</center>

**rm -rf** adalah suatu perintah untuk menghapus suatu directory beserta isi dari directory tersebut. Sekarang kita coba hapus directory **wordpress** yang tadi sudah kita extract sebelumnya.

```shell
rm -rf wordpress
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/shell30.png')} height="400px"/>
</center>

