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
<img alt="image1" src={useBaseUrl('img/docs/image-3.png')} height="400px"/>
</center>

Jadi kurang lebih cara kerja CI/CD seperti ini :

Programmer yang telah menyelesaikan aplikasi yang telah dibuat, maka akan melakukan commit. **Commit** adalah proses penyimpanan code aplikasi ke repository / server. 

Kemudian, code tersebut akan diteruskan ke sebuah tools CI/CD salah satunya adalah **Jenkins**. Pada proses tersebut akan melakukan proses build dan test pengecekan code apakah ada bug atau tidak. 

Jika proses tersebut berjalan dengan lancar maka akan diteruskan ke server hingga dapat di akses oleh pengguna, tapi jika terdapat bug akan ada pemberitahuan ke email.

Dan semua proses tersebut akan berulang-ulang secara otomatis.