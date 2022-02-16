---
sidebar_position: 1
---

# 1. CI/CD

## 1.1 Apa itu CI/CD?

import useBaseUrl from '@docusaurus/useBaseUrl';

CI/CD atau **Continuous Integration** dan **Continuous Deployment** merupakan metode untuk mengirimkan perubahan code secara terus menerus hingga aplikasi dapat release ke publik dengan otomatis.

- **Continuous integration** merupakan proses otomatis untuk memastikan semua code sudah berjalan dengan baik, jika terjadi error maka proses tersebut akan diulangi dari awal hingga code tersebut sudah tidak ada error.
- **Continuous deployment** merupakan proses otomatis agar aplikasi yang telah siap di kirim ke server hingga aplikasi dapat diakses secara public.

## 1.2 Kenapa menggunakan CI/CD

### 1. Tanpa menggunakan CI/CD

- Proses penyebaran aplikasi dilakukan secara manual
- Risiko aplikasi tidak berfungsi ketika production lebih besar
- Rollback ke versi sebelumnya akan lebih sulit jika dilakukan manual

### 2. Jika menggunakan CI/CD

- Dapat menyebarkan aplikasi sesuai dengan permintaan
- Dapat mengurangi risiko aplikasi tidak berfungsi ketika production
- Dapat dengan mudah di rollback ke versi sebelumnya jika terjadi error

### 3. CI/CD Tools

Berikut adalah beberapa Tools yang dapat digunakan untuk CI/CD :

- Github Actions
- GitLab CI/CD
- Bitbucket Bamboo
- Jenkins
