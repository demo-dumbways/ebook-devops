---
sidebar_position: 8
---

# 8. Git add and Commit

import useBaseUrl from '@docusaurus/useBaseUrl';

Sebelum kita lebih jauh lagi membahas tentang `git` ini. Kita perlu mengetahui 3 kondisi file dalam git.

## Git Condition :
Berikut adalah beberapa tahapan di `git`: 

### 1. Modified
**Modified** adalah tahapan dimana revisi atau perubahan sudah dilakukan, tetapi belum ditandai dan belum disimpan ke dalam database git.

### 2. Staged
**Staged** adalah kondisi dimana revisi sudah di tandai, tetapi belum disimpan di database git. Untuk mengubah kondisi dari modified ke staged gunakan perintah `git add`

### 3. Commited
**Commited** adalah kondisi dimana revisi sudah disimpan dalam database git. Untuk mengubah kondisi dari staged ke commited gunakan perintah `git commit`

## Git add
Sebelumnya masuk ke materi ini kita sudah melakukan kondisi pertama yaitu **modified**, dengan membuat beberapa file yaitu `file1`, `file2`, dan `file3`. Sekarang kita akan menggunakan perintah `git add`.

### 1. git add file1

```shell
git add file1
```
keterangan : akan melakukan stage pada `file1`

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/git16.png')} height="500px"/>
  </center>

### 2. git add *.html

```shell
git add *.html
```
keterangan : akan melakukan stage pada semua file yang berakhiran `.html`

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/git17.png')} height="420px"/>
  </center>

### 3. git add .

```shell
git add .
```
keterangan : akan melakukan stage pada semua file

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/git18.png')} height="500px"/>
  </center>

## Git commit  
Sekarang kita berada pada tahap **staged**, yang terakhir adalah **commit**.
### 1. git commit 
Untuk membuat commit kalian harus menjalankan perintah `git commit`

```shell
git commit -m "pesan commit yang ingin kalian buat"
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/git19.png')} height="500px"/>
  </center>


Jika sudah selesai maka semua perubahan akan tersimpan pada database git. Dan ketika kalian menjalankan perintah `git status` maka akan muncul notifikasi seperti ini `nothing to commit, working directory clean`.



