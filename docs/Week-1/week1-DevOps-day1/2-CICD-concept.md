---
sidebar_position: 2
---

# 2. CI/CD Concept

import useBaseUrl from '@docusaurus/useBaseUrl';

**CI/CD** adalah kepanjangan dari **Continuous Integration** dan **Continuous Deployment**. Merupakan metode untuk mengirimkan perubahan code secara terus menerus hingga aplikasi dapat release ke publik dengan otomatis.

Lebih spesifik lagi : 

**Continuous Integration** merupakan serangkaian proses otomatisasi untuk developer ketika melakukan perubahan code agar dapat diperiksa lebih dahulu sebelum masuk ke tahap continuous deployment. Hal ini diperlukan agar dapat mengetahui terjadinya error lebih cepat.

**Ilustrasi Continous Integration** 
Gambaran ilustrasi untuk gambar di atas kurang lebih seperti ini, Jadi para Developer sedang membuat suatu code untuk membuat suatu aplikasi, jika para code yang di buat oleh para Developer sudah selesai makan akan di lanjutkan ke tahapan **continous integration** nah di bagian ini si aplikasi akan di cek apakah sudah sesuai dengan yang di harapkan lalu juga di cek nih apakah ada bug di aplikasi yang sudah di buat oleh para Developer. Nah jika misalkan terjadi suatu bug maupun aplikasinya ternyata belum seseuai dengan yang di harapkan, maka si aplikasi akan di kembalikan ke para Developer untuk meng-fix kan bug ataupun menambahkan fitur yang kurang agar bisa sesuai dengan expetasi yang di harapakan. Nah jika si aplikasi ternyata saat di tes tidak ada bug dan aplikasi sudah sesuai dengan yang di harapkan maka si aplikasi ini sudah siap untuk di lanjutkan ke tahap **Deployment**.  

**Continuous Deployment** merupakan proses otomatisasi agar aplikasi yang telah siap di deploy ke server dapat diteruskan hingga aplikasi dapat diakses secara public.

**Ilustrasi Continous Deploment**
Gambaran untuk ilustrasi untuk gambar di atas kurang lebih seperti ini, Melanjutkan ilustrasi continous integration tadi nah jika aplikasi sudah tidak ada bug dan sesuai expetasi yang di harapkan, maka si aplikasi ini sudah siap untuk di deploy ke beberapa server. 

**Kelebihan Menggunakan CI/CD** : 
1. Dapat menyebarkan aplikasi sesuai dengan permintaan.
2. Dapat mengurangi risiko aplikasi tidak berfungsi ketika production.
3. Dapat dengan mudah di rollback ke versi sebelumnya jika terjadi error.

**CI/CD Tools**
1. Jenkins.
2. Bitbucket pipelines.
3. Github actions.
4. Gitlab CI.
5. Circle CI.

**CI/CD Workflow**
<img alt="image1" src={useBaseUrl('img/docs/image-1.png')} height="300px"/>
