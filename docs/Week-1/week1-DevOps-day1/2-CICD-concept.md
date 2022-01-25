---
sidebar_position: 2
---

# 2. CI/CD Concept

import useBaseUrl from '@docusaurus/useBaseUrl';

**CI/CD** adalah kepanjangan dari **Continuous Integration** dan **Continuous Deployment**. Merupakan metode untuk mengirimkan perubahan code secara terus menerus hingga aplikasi dapat release ke publik dengan otomatis.

Lebih spesifik lagi : 

**Continuous Integration** merupakan serangkaian proses otomatisasi untuk developer ketika melakukan perubahan code agar dapat diperiksa lebih dahulu sebelum masuk ke tahap continuous deployment. Hal ini diperlukan agar dapat mengetahui terjadinya error lebih cepat.

**Continuous deployment** merupakan proses otomatisasi agar aplikasi yang telah siap di deploy ke server dapat diteruskan hingga aplikasi dapat diakses secara public.

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
