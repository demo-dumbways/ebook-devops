---
sidebar_position: 8
---

# 8. Git Remote

import useBaseUrl from '@docusaurus/useBaseUrl';

Pada proyek pengembangan aplikasi, kita tidak akan bekerja sendiri. Perlu adanya server untuk menyimpan semua perubahan yang telah dilakukan agar orang lain juga dapat berkontribusi terhadap pengembangan.

Dimanakah repository tersimpan? Repository akan disimpan pada layanan internet, berikut adalah beberapa layanan yang paling banyak digunakan di dunia :
- GitHub
- GitLab
- Bitbucket

### Studycase :
Kita akan melakukan remote pada layanan GitHub, hal yang perlu diperhatikan adalah :
- Registrasi pada halaman github.com
- Buat sebuah repository dengan nama Dumbways.id
- Masukkan deskripsi repository misalkan `Saya belajar Version Control System (Git)`
- Tentukan repository public atau private
- Kemudian klik create repository
- Add git remote to your local server

### 1. Create Github account
Untuk membuat akun github bisa click link dibawah ini :

**LINK : [Github.com](https://github.com/)**
   <center>
   <img alt="image1" src={useBaseUrl('img/docs/image-33.png')} height="330px"/>
   </center>

### 2. Make Repository
**Repository** adalah suatu penyimpanan file project. dimana kamu bisa menyimpan apapun yang berkaitan dengan project kalian, seperti code, gambar, ataupun audio. repo sendiri bertempat di penyimpanan atau storage github atau repository local di komputer anda.
   <center>
   <img alt="image1" src={useBaseUrl('img/docs/git20.png')} height="330px"/>
   </center>

Pada bagian ini, kita dapat mengisi sendiri melalui penjelasan singkat dibawah ini:

- **repository name** adalah kolom untuk memberikan nama pada repository yang ingin kalian buat.
- **description** adalah kolom untuk mendeskripsikan repo yang ingin dibuat. Sifatnya opsional yaitu boleh diisi atau tidak.
- **Visibility** adalah untuk memilih repository yang ingin kalian buat itu bersifat apa. lalu terdapat dua opsi penampilan repo yaitu "public" dan "private". Pilih public jika reopository kalian ingin dapat di akses oleh pengguna lain/pilih private jika repository yang kalian buat ini hanya dapat di akses oleh kalian sendiri.
- Jika merasa sudah sesuai kalian bisa langsung tekan saja **create repository** di bagian paling bawah.

### 3. Add git remote
Copy yang sudah disediakan Github, jangan lupa untuk memilih bagian **SSH** karena kita menggunakan **SSH** untuk mengkoneksikan local kita dengan **Github**.
   <center>
   <img alt="image1" src={useBaseUrl('img/docs/git21.png')} height="330px"/>
   </center>

```shell
git remote add origin git@github.com:demo-dumbways/Dumbways.id.git
```
   <center>
   <img alt="image1" src={useBaseUrl('img/docs/git22.png')} height="400px"/>
   </center>

### 4. Check remote
Untuk melihat remote yang kita gunakan kita bisa menggunakan perintah berikut :

```shell
git remote -v
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/git23.png')} height="400px"/>
</center>