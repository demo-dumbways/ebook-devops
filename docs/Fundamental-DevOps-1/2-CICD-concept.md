---
sidebar_position: 2
---

# 2. CI/CD Concept

import useBaseUrl from '@docusaurus/useBaseUrl';

**CI/CD** adalah kepanjangan dari **Continuous Integration** dan **Continuous Deployment**. Merupakan metode untuk mengirimkan perubahan code secara terus menerus hingga aplikasi dapat release ke publik dengan otomatis.

Lebih spesifik lagi : 

**Continuous Integration** Continuous integration (CI) adalah pengintegrasian kode ke dalam repositori kode kemudian menjalankan pengujian secara otomatis, cepat, dan sering. Kamu dapat melakukan CI ini dengan menggunakan perintah commit.

**Continuous Deployment** adalah praktik yang dilakukan setelah proses CI selesai dan seluruh kode berhasil terintegrasi, sehingga aplikasi bisa dibangun lalu dirilis secara otomatis.

**Manfaat dari CI/CD** : 
1. Dapat menyebarkan aplikasi sesuai dengan permintaan.
2. Dapat mengurangi risiko aplikasi tidak berfungsi ketika production.
3. Dapat dengan mudah di rollback ke versi sebelumnya jika terjadi error.
4. Mendapat feedback lebih cepat.
5. Dapat mendeteksi bug lebih cepat.

**CI/CD Tools**
1. Jenkins.
2. Bitbucket pipelines.
3. Github actions.
4. Gitlab CI.
5. Circle CI.

**Workflow**
<center>
<img alt="image1" src={useBaseUrl('img/docs/image-3.png')} height="250px"/>
</center>

Jadi kurang lebih cara kerja CI/CD seperti ini :

Para Developer (Programmer) yang telah menyelesaikan coding-an mereka, mereka akan melakukan yang namanya **commit**, nah commit ini apa **commit ini adalah proses penyimpanan coding-an para Developer**. Setelah itu coding-an para Developer akan di simpan ke sebuah Platrform yang bernama GIT. **Git ini adalah sebuah platfform yang memudahkan para Developer untuk menyimpan code yang sudah mereka buat**. Setelah itu akan di teruskan ke sebuah tools CI/CD kita ambil contoh disini adalah **Jenkins**. Nah **Jenkins ini adalah sebuah tools yang berfungsi untuk mengecek code yang sudah dibuat oleh para Developer apakah ada bug atau tidak**. Jika ada bug maka si Jenkins ini akan memberitahu nih ternyata di coding-an yang sudah di buat oleh para Developer ini ada bug. Lalu jika ternyata tidak ada bug si Jenkins ini akan melakukan Deployment ke server agar aplikasi yang sudah dibangun oleh para Developer itu tadi, bisa di gunakan oleh user.