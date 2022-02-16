---
sidebar_position: 7
---

# 7. Git Ignore

import useBaseUrl from '@docusaurus/useBaseUrl';

## 7.1 Apa itu .gitignore?

**.gitignore** adalah sebuah file yang berisi daftar nama-nama file dan direktori yang akan **diabaikan/diasingkan** oleh git. Perubahan apapun yang kita lakukan terhadap file dan direktori yang sudah masuk ke dalam daftar **.gitignore** tidak akan dicatat oleh git.

## 7.2 Mengapa memerlukan .gitignore?

Karena pada kenyataannya di sebagian proyek terdapat file yang dihasilkan saat menjalankan / perlu menginstal beberapa komponen tambahan agar aplikasi dapat berjalan dan biasanya file tidak ada gunanya karena dapat di unduh ulang.

Kita ambil contoh saja dalam proyek `node.js` ada folder bernama `node_modules` yang berisi semua paket external yang perlu dijalankan oleh kode kalian. Kalian dapat menghapus file `node_modules` ini dan dapat membangunnya kembali dengan menjalankan perintah `npm install`.

Berikut adalah cara pembuatan **.gitignore**:

- Pertama-tama disini kalian coba buat beberapa file

  ```shell
  touch file1 file2 file3
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/git11.png')} height="500px"/>
  </center>

- Setelah itu kita coba cek menggunakan perintah `git status`

  ```shell
  git status
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/git12.png')} height="500px"/>
  </center>

  Disini kita dapat melihat masih ada `file1`, `file2`, dan `file3`.

- Sekarang kita akan coba untuk **mengabaikan/mengasingkan** `file3` yang sudah kita buat sebelumnya.
- Disini kita buat terlebih dahulu file dengan nama `.gitignore`.

  ```shell
  touch .gitignore
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/git13.png')} height="500px"/>
  </center>

- Selanjutnya sekarang kita masukan nama file yang ingin kita **abaikan/asingkan** `(file3)`.

  ```shell
  sudo nano .gitignore
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/git14.png')} height="500px"/>
  </center>

- Jika sudah sekarang kita cek lagi apakah `file3` masih terbaca atau tidak dengan menggunakan perintah `git status`.

  ```shell
  git status
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/git15.png')} height="500px"/>
  </center>

  Kalau kita lihat sekarang `file3` sudah tidak terbaca lagi mengapa? Karena kita sudah mengasingkan `file3` di file `.gitignore`.
