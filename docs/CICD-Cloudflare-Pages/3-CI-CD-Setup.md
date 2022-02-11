---
sidebar_position: 3
---

# 3. Set-Up CI/CD Sederhana

import useBaseUrl from '@docusaurus/useBaseUrl';

Selain menggunakan tools CI/CD yang telah disebutkan sebelumnya, kita akan mencoba melakukan konfigurasi sederhana untuk memahami konsep dan cara kerja CI/CD menggunakan **Cloudflare Pages**.

## CI/CD Set-Up with Cloudflare
### 1. Registrasi
Pastikan kalian sudah melakukan register ke https://cloudflare.com, Jika kalian belum mempunyai akun **Cloudflare** kalian bisa melakukan registrasi dengan klik link dibawah ini.

**LINK Cloudflare : [Registrasi](https://dash.cloudflare.com/sign-up)**

<center>
<img alt="image1" src={useBaseUrl('img/docs/cicd1.png')} height="500px"/>
</center>

### 2. Cloudflare pages
- Jika kalian sudah selesai melakukan registrasi kalian bisa masuk ke menu **pages** untuk membuat project baru.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd2.png')} height="500px"/>
    </center>

- Selanjutnya Tekan bagian **Connect to GitHub**, supaya repository di github kita terdeteksi ke **Cloudflare Pages**

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd3.png')} height="500px"/>
    </center>

- Pilih akun yang sesuai. Misalkan saya menggunakan akun pribadi yang bernama demo-dumbways dan pilih satu repository.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd4.png')} height="500px"/>
    </center>

- Jika sudah kalian dapat memilih semua repository maupun salah satu repository saja. Dalam hal ini kita hanya menghubungkan **cloudflare pages** ke salah satu repository saja.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd5.png')} height="500px"/>
    </center>

- kemudian akan menampilkan halaman berikut, dan bisa klik `begin setup` untuk proses konfigurasinya. 

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd6.png')} height="500px"/>
    </center>

- Pastikan untuk mengisi nama dan branch yang digunakan, kemudian pada bagian **build settings** pilih **framework** yang digunakan kemudian pastikan untuk memasukkan build commandnya. Jika sudah sesuai langsung saja klik `Save and Deploy`.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd7.png')} height="500px"/>
    </center>

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd8.png')} height="500px"/>
    </center>
- Setelah itu kita tunggu saja sampai proses build selesai.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd9.png')} height="500px"/>
    </center>

- Jika proses build berhasil maka akan terlihat seperti berikut.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd10.png')} height="500px"/>
    </center>

- Sekarang kita coba akses aplikasi yang sudah kita deploy menggunakan **cloudflare** ini dengan url yang ada di sebelah `Domains`.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd11.png')} height="500px"/>
    </center>

- Berikut adalah website yang telah berhasil dijalankan ke server **Cloudflare Pages**.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd12.png')} height="500px"/>
    </center>

### 3. Update code
Sekarang kita akan mencoba mempraktekkan bagaimana cara kerja dari **CI/CD**, setiap ada perubahan code maka code tersebut akan dikirimkan ke server **Cloudflare Pages**.

- Sekarang kita akan mencoba untuk melakukan perubahan code pada bagian **title**, Kita coba ubah pada bagian `<title> ... </title>`, dimaksudkan untuk mengetahui apakah proses CI/CD berhasil atau tidak.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd13.png')} height="500px"/>
    </center>

- Selanjutnya kita coba lihat di **Cloudflare pages** kita, disini **Cloudflare** secara otomatis melakukan build ulang, kenapa? karena sebelumnya kita sudah melakukan suatu perubahan di bagian `title` tadi. Selanjutnya kita tunggu saja sampai proses build selesai.

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd14.png')} height="500px"/>
    </center>

- Jika sudah selesai dan proses build telah berhasil, maka akan berubah seperti di bawah ini. Pada bagian title yang sebelumnya **Dumbflix - Fadhil Darma Putera Z** telah menjadi **Dumbflix - Rizqy Alvindra**

    <center>
    <img alt="image1" src={useBaseUrl('img/docs/cicd15.png')} height="500px"/>
    </center>