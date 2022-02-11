---
sidebar_position: 2
---

### 2. Go

import useBaseUrl from '@docusaurus/useBaseUrl';

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


   