---
sidebar_position: 1
---

# 1. Application
import useBaseUrl from '@docusaurus/useBaseUrl';

**Application** adalah sebuah perangkat lunak komputer yang melakukan fungsi spesifik secara langsung untuk pengguna akhir. Aplikasi dapat berjalan secara mandiri atau secara bersamaan dengan sekelompok program.

## Kenapa mempelajari aplikasi ?
Berikut ini adalah beberapa alasan harus mempelajari aplikasi:
- Setiap bahasa pemrograman memiliki cara berbeda untuk setupnya
- Setiap aplikasi memiliki cara berbeda untuk menjalankannya

## Make Simple Application :
Kita akan mencoba untuk membuat beberapa simple apllikasi.

### 1. Node.Js

- Pertama-tama kita harus meng-install terlebih engine-nya dahulu. Untuk instalasi kalian bisa menggunakan beberapa perintah dibawah ini.

 ```shell
 curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
 ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/tun2.png')} height="400px"/>
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
  <img alt="image1" src={useBaseUrl('img/docs/app1.png')} height="400px"/>
  </center>

  keterangan : perintah di atas berguna untuk menginstall **node.js** dengan versi 14. Jika kalian ingin menggunakan **node.js** dengan`version 14`, maka Jalankan perintah `nvm install 14`.

  ```shell
  nvm use 16
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app2.png')} height="400px"/>
  </center>

  keterangan : Untuk menggunakan node.js dengan versi 14

  Jika tahapan di atas sudah kalian lakukan, maka kalian sudah berhasil untuk melakukan instalasi **node.js**. Untuk melakukan pengecekan kalian bisa menggunakan perintah di bawah ini.

  ```shell
  node -v
  ```

  ```shell
  npm -v
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app3.png')} height="400px"/>
  </center>

- Selanjutnya kita akan menjalankan perintah `npm init` gunanya untuk mengisiasi project, Hasil dari kalian menjalankan perintah akan membuat file baru dengan nama **package.json**, **package.json** ini berisikan isi informasi dari aplikasi yang akan kalian buat.

  ```shell
  npm init -y
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app4.png')} height="400px"/>
  </center>

- Selanjutnya kita akan menginstall **Express JS**. **Express JS** adalah framework dari NodeJS yang dirancang secara fleksibel dan sederhana untuk membantu tahap pengembangan aplikasi back end. Menginstall **express js** dapat dilakukan menggunakan **NPM** dengan perintah berikut:

```shell
npm install express --save
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app5.png')} height="400px"/>
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
  <img alt="image1" src={useBaseUrl('img/docs/app6.png')} height="400px"/>
  </center>

- Jika sudah sekarang kita akan coba untuk menjalankan aplikasi sederhana yang sudah kita buat. Untuk menjalankan dapat menggunakan perintah berikut ini.

```shell
node index.js
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app7.png')} height="400px"/>
  </center>

keterangan : untuk keluar bisa menggunakan `CTRL + X`

- Sekarang coba akses Web.Browser kalian setelah itu kalian coba akses dengan `localhost:3000`

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app8.png')} height="400px"/>
  </center>

### 2. Python3
- Pertama-tama kita harus install terlebih dahulu **Pyhton3**. Untuk instalasi ikuti beberapa perintah di bawah ini.

```shell
sudo apt update; sudo apt upgrade
```

- Python3 sudah ada secara default, untuk melakukan pengecekan jalankan perintah berikut.

```shell
python3 -v
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app9.png')} height="400px"/>
  </center>

- Sekarang kita install package manager dari python3. Kalian dapat menggunakan perintah berikut ini.

```shell
sudo apt install python3-pip
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app10.png')} height="420px"/>
  </center>

```shell
pip install flask
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app11.png')} height="400px"/>
  </center>

  **PIP** adalah sebuah package management system yang biasa digunakan untuk mengatur dan menginstall **package yang berisi modul-modul Python**. PIP digunakan untuk menginstall **Flask** karena Flask ditulis dan dikembangkan dengan bahasa dan modul-modul pemrograman **Python**. Dengan menggunakan PIP, semua hal yang dibutuhkan untuk instalasi Flask akan diunduh dan dipasang dalam satu perintah.

- Sekarang kita akan membuat aplikasi sederhana menggunakan **Python3**. 
- Kalian buat terlebih dahulu file dengan nama index.py. Lalu masukan script dibawah ini.

```shell
nano index.py
```

  ```py title="index.py"
  from flask import Flask
  app = Flask(__name__)
  @app.route("/")
  def helloworld():
      return "Hello World"
  if __name__ == "__main__":
      app.run()
  ```

- Jika sudah sekarang jalankan aplikasi dengan menggunakan perintah berikut ini.
  ```shell
  python3 index.py
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app12.png')} height="400px"/>
  </center>
  
  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app13.png')} height="400px"/>
  </center>

- Sekarang coba akses Web.Browser kalian setelah itu kalian coba akses dengan `localhost:5000`

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app14.png')} height="400px"/>
  </center>

### 3. Go
- Pertama-tama sama seperti sebelumnya, kita harus mendownload engine-nya terlebih dahulu.

```shell
wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz && sudo su
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app15.png')} height="400px"/>
  </center>

```shell
rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz && exit
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app16.png')} height="400px"/>
  </center>

-  Selanjutnya masukkan path go pada `.bashrc`
  ```shell
  sudo nano .bashrc
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app17.png')} height="400px"/>
  </center>

  ```shell
  export PATH=$PATH:/usr/local/go/bin
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app18.png')} height="400px"/>
  </center>

- Jika sudah sekarang dapat verifikasi go dengan cara berikut.
  ```shell
  go version
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app19.png')} height="400px"/>
  </center>

- Sekarang kita akan membuat aplikasi sederhana menggunakan `go`. Kalian dapat menjalankan beberapa perintah berikut ini.
- Buat sebuah file dengan nama `index.go`.

  ```shell
  nano index.go
  ```

- Setelah itu masukkan script dibawah ini.

  ```go title="index.go"
  package main

  import "fmt"

  func main() {
      fmt.Println("Hello World!")
  }
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app20.png')} height="400px"/>
  </center>


- Sekarang jalankan aplikasi go dengan menggunakan perintah berikut.
  ```shell
  go run index.go
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app21.png')} height="400px"/>
  </center>

- Jika aplikasi kalian ingin di build, maka jalankan perintah berikut ini.

  ```shell
  go build index.go
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app22.png')} height="400px"/>
  </center>

- Jika sudah jalankan aplikasi dengan menggunakan perintah berikut.
  ```shell
  ./index
  ```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app23.png')} height="400px"/>
  </center>


   