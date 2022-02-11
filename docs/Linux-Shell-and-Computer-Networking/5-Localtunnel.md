---
sidebar_position: 5
---

# 5. Localtunnel

import useBaseUrl from '@docusaurus/useBaseUrl';

## 5.1 Apa itu Localtunnel?
**Localtunnel** adalah sebuah tools yang memungkinkan kita untuk berbagi layanan website dari lokal komputer ke publik dengan url akses yang disediakan oleh localtunnel.

**Ilustrasi bagaimana cara Localtunnel bekerja**

<center>
<img alt="image1" src={useBaseUrl('img/docs/localtunnel.png')} height="300px"/>
</center>

## 5.2 Kenapa Localtunnel ?
- Kita dapat membuat aplikasi web dapat diakses secara publik.
- Tidak perlu meletakkan web tersebut ke server online.
- Tidak perlu membeli domain.

## 5.3 Bagaimana Menggunakan Localtunnel?

Kita akan mencoba untuk melakukan konfigurasi localtunnel agar server kita dapat di akses secara publik. Berikut adalah step by step cara menggunakannya:

```shell
git clone https://github.com/dumbwaysdev/dumbflix-frontend.git
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun5.png')} height="400px"/>
</center>

Jika sudah masuk ke directory yang sudah kalian clone, setelah itu jalankan perintah seperti dibawah ini.

```shell
cd dumbflix-frontend
```

```shell
npm install
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/tun6.png')} height="400px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun7.png')} height="400px"/>
</center>

Jika tahapan di atas sudah selesai maka jalankan aplikasi dengan menggunakan perintah di bawah ini.

```shell
npm start
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun8.png')} height="400px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun10.png')} height="400px"/>
</center>

Jika tahapan di atas sudah selesai kalian jalankan maka aplikasi sekarang sudah berjalan. Step selanjutnya adalah coba kalian **buka web browser** kalian lalu masukkan **IP dari server kalian** setelah masukan port dari aplikasi, contoh : 192.168.64.6:3000 

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun9.png')} height="400px"/>
</center>

Sekarang kita akan coba untuk menjalankan aplikasi menggunakan **Localtunnel** agar mendapatkan random **url** yang bisa di akses oleh publik. Untuk menjalankan localtunnel bisa menggunakan perintah dibawah ini.

```shell
lt --port 3000
```

Karena aplikasi ini berjalan di **port 3000** maka dibagian **lt --port(port aplikasi)**, masukkan sesuai dengan aplikasi kalian.

Jika kalian sudah menjalankan perintah sebelumnya maka nanti akan muncul sebuah url yang ada di terminal kalian. Kurang lebih seperti gambar di bawah ini

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun11.png')} height="400px"/>
</center>

Jika sudah copy saja **url** yang ada di terminal kalian. Jika sudah buka **web browser** kalian setelah itu paste url yang sudah kalian copy tadi. Nantinya kalian akan di arahkan ke bagian seperti di bawah ini.

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun12.png')} height="400px"/>
</center>

Jika sudah maka langsung saja klik di bagian **Click to continue**. Maka nantinya kalian akan di arahkan ke aplikasi kalian.

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun13.png')} height="400px"/>
</center>