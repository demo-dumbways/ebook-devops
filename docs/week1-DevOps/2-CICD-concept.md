---
sidebar_position: 2
---

# 2. CI/CD Concept

import useBaseUrl from '@docusaurus/useBaseUrl';

## Apa itu CI/CD ?
**CI/CD** adalah kepanjangan dari **Continuous Integration** dan **Continuous Deployment**. Merupakan metode untuk mengirimkan perubahan code secara terus menerus hingga aplikasi dapat release ke publik dengan otomatis.

Lebih spesifik lagi : 

**Continuous Integration** merupakan serangkaian proses otomatisasi untuk developer ketika melakukan perubahan code agar dapat diperiksa lebih dahulu sebelum masuk ke tahap continuous deployment. Hal ini diperlukan agar dapat mengetahui terjadinya error lebih cepat.

**Continuous deployment** merupakan proses otomatisasi agar aplikasi yang telah siap di deploy ke server dapat diteruskan hingga aplikasi dapat diakses secara public.

**Kelebihan Menggunakan CI/CD** : 
1. Dapat menyebarkan aplikasi sesuai dengan permintaan
2. Dapat mengurangi risiko aplikasi tidak berfungsi ketika production
3. Dapat dengan mudah di rollback ke versi sebelumnya jika terjadi error

<img alt="image1" src={useBaseUrl('img/docs/image-3.png')} height="300px"/>

<img alt="image1" src={useBaseUrl('img/docs/image-4.png')} height="300px"/>
