---
sidebar_position: 3
---

### 3. Python3

**Python** adalah Python merupakan bahasa pemrograman tingkat tinggi yang diracik oleh Guido van Rossum. Python banyak digunakan untuk membuat berbagai macam program, seperti: program CLI, Program GUI (desktop), Aplikasi Mobile, Web, IoT, Game, Program untuk Hacking.

import useBaseUrl from '@docusaurus/useBaseUrl';

- Pertama-tama kita harus install terlebih dahulu **Pyhton3**. Untuk instalasi ikuti beberapa perintah di bawah ini.

```shell
sudo apt update; sudo apt upgrade
```

- Python3 sudah ada secara default, untuk melakukan pengecekan jalankan perintah berikut.

```shell
python3 -v
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app9.png')} height="500px"/>
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
  <img alt="image1" src={useBaseUrl('img/docs/app11.png')} height="500px"/>
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
  <img alt="image1" src={useBaseUrl('img/docs/app12.png')} height="500px"/>
  </center>

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app13.png')} height="500px"/>
  </center>

- Sekarang coba akses web browser kalian setelah itu kalian coba akses dengan `localhost:5000`

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/app14.png')} height="500px"/>
  </center>
