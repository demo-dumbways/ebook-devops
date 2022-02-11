---
sidebar_position: 13
---

# 12. Git Merge

import useBaseUrl from '@docusaurus/useBaseUrl';

**Merge** adalah suatu perintah dalam **git** untuk membuat branch yang bercabang menjadi satu kembali atau dengan kata lain mengintegrasikan kembali branch tersebut menjadi satu. **Merge** akan mengombinasikan beberapa tahapan commits menjadi satu branch yang terunifikasi.

Sekarang kita coba praktekkan :

<center>
<img alt="image1" src={useBaseUrl('img/docs/git=.png')} height="500px"/>
</center>

- Disini kalau kita lihat dari gambar di atas saya sedang berada di dalam branch **master**.
- Selanjutnya saya melakukan perubahan di beberapa file yaitu **file.html**, **file1**, **file2**.
- Setelah itu kita lakukan `git add` dan `git commit` untuk melakukan penyimpanan.
- Selanjutnya saya berpindah branch dari **master** ke **development**
- Jika sudah pindah ke dalam branch **development**, selanjutnya kita akan melakukan perintah git `merge` untuk menggabungkan branch **master** dengan branch **development**, untuk perintah `git merge` kalian dapat menggunakan perintah di bawah ini.

```shell
git merge (the name of the file you want to merge)
```
