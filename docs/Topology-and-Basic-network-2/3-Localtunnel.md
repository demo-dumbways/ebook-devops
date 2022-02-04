---
sidebar_position: 3
---

# 3. Localtunnel

import useBaseUrl from '@docusaurus/useBaseUrl';

**Localtunnel** adalah sebuah tools yang memungkinkan kita untuk berbagi layanan website dari lokal komputer ke publik dengan url akses yang disediakan oleh localtunnel.

**Ilustrasi bagaimana cara Localtunnel bekerja**

<center>
<img alt="image1" src={useBaseUrl('img/docs/localtunnel.png')} height="300px"/>
</center>

## Kenapa Localtunnel ?
- Kita dapat membuat aplikasi web dapat diakses secara publik.
- Tidak perlu meletakkan web tersebut ke server online.
- Tidak perlu membeli domain.

### 1. Install node.js

- Install terlebih dahulu node.js menggunakan nvm, Untuk installasi bisa mengikuti step by step dibawah.

```
sudo apt install curl
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/tun1.png')} height="400px"/>
</center>

```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun2.png')} height="400px"/>
</center>

```shell
exec bash
```

```shell
nvm install 14
```

Jika kalian sudah melakukan step by step diatas maka instalasi sudah selesai. Untuk mengecek Versi dari **nvm**, **node.js**, dan **npm** yang kita gunakan bisa menggunakan perintah di bawah.

```shell
nvm -v
```

```shell
node -v
```

```shell
npm -v
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun3.png')} height="400px"/>
</center>

### 2. Localtunnel Installation

```shell
npm install -g localtunnel
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/tun4.png')} height="400px"/>
</center>

### 3. How to use Localtunnel
Disini kita akan coba untuk menjalankan suatu aplikasi. Untuk bagaimana cara menggunakan localtunnel ini bisa ikuti step by step dibawah ini.

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