---
sidebar_position: 1
---

## Make Simple Application :
Kita akan mencoba untuk membuat beberapa simple apllikasi.

### 1. Node.Js

import useBaseUrl from '@docusaurus/useBaseUrl';

- Pertama-tama kita harus meng-install terlebih engine-nya dahulu. Untuk instalasi kalian bisa menggunakan beberapa perintah dibawah ini.

 ```shell
 curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
 ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tun2.png')} height="500px"/>
  </center>

  keterangan : disini kita menggunakan `nvm` 

  `nvm` merupakan singkatan dari **Node Version Manager**. `nvm` adalah sebuah program yang akan membantu kita untuk menggunakan lebih dari satu versi Nodejs di dalam satu komputer.

  ```shell
  exec bash
  ```
  
  keterangan : Jika nvm belum terdeteksi gunakan perintah di atas ini

  ```shell
  nvm install 16
  ```
  
  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app1.png')} height="500px"/>
  </center>

  keterangan : perintah di atas berguna untuk menginstall **node.js** dengan versi 16. Jika kalian ingin menggunakan **node.js** dengan`version 14`, maka Jalankan perintah `nvm install 14`.

  ```shell
  nvm use 16
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app2.png')} height="500px"/>
  </center>

  keterangan : Untuk menggunakan node.js dengan versi 16

  Jika tahapan di atas sudah kalian lakukan, maka kalian sudah berhasil untuk melakukan instalasi **node.js**. Untuk melakukan pengecekan kalian bisa menggunakan perintah di bawah ini.

  ```shell
  node -v
  ```

  ```shell
  npm -v
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app3.png')} height="500px"/>
  </center>

- Selanjutnya kita akan menjalankan perintah `npm init` gunanya untuk mengisiasi project, Hasil dari kalian menjalankan perintah akan membuat file baru dengan nama **package.json**, **package.json** ini berisikan isi informasi dari aplikasi yang akan kalian buat.

  ```shell
  npm init -y
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app4.png')} height="500px"/>
  </center>

- Selanjutnya kita akan menginstall **Express JS**. **Express JS** adalah framework dari NodeJS yang dirancang secara fleksibel dan sederhana untuk membantu tahap pengembangan aplikasi back end. Menginstall **express js** dapat dilakukan menggunakan **NPM** dengan perintah berikut:

```shell
npm install express --save
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app5.png')} height="500px"/>
  </center>

- Jika sudah buat file dengan nama `index.js`, lalu masukan script dibawah ini
```shell
nano index.js
``` 

```js title="index.js"
const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => {
  res.send('Hello World!')
})

app.listen(port, () => {
  console.log(`Example app listening on port ${port}`)
})
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app6.png')} height="500px"/>
  </center>

- Jika sudah sekarang kita akan coba untuk menjalankan aplikasi sederhana yang sudah kita buat. Untuk menjalankan dapat menggunakan perintah berikut ini.

```shell
node index.js
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app7.png')} height="500px"/>
  </center>

keterangan : untuk keluar bisa menggunakan `CTRL + X`

- Sekarang coba akses web browser kalian setelah itu kalian coba akses dengan `localhost:3000`

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app8.png')} height="500px"/>
  </center>
