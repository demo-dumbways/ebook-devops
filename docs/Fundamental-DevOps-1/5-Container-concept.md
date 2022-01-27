---
sidebar_position: 5
---

# 5. Container 

import useBaseUrl from '@docusaurus/useBaseUrl';

**Container** adalah sebuah paket aplikasi yang dikemas dengan dependensi-dependensinya sehingga aplikasi dapat berjalan dengan cepat tanpa perlu mengkonfigurasi sebuah environment tertentu pada sistem operasi.
Dengan teknologi **container** kita dapat menjalankan aplikasi yang sudah berbentuk container tersebut di sistem operasi Windows ataupun Linux.

Berikut adalah Gambaran bagaimana cara Container bekerja:
   <img alt="image1" src={useBaseUrl('img/docs/image-10.png')} height="275px"/>

Infrastruktur dari container ini sendiri kurang lebih seperti ini. Jadi di bawahnya ini ada infrastruktur lalu di atas infrastruktur ini kalian install sebuah sistem operasi, Jadi sistem operasinya ini bisa ubuntu maupun windows terserah kalian nantinya. nah kemudian di atas sistem operasi ini kalian perlu install aplikasi yang namanya **Docker**. Docker ini adalah suatu tools yang mendukung container. jadi kalau misalkan ingin menjalakan sebuah container kalian butuh Docker. lalu di atas Docker ini kalian bisa membuat sebuah aplikasi dalam bentuk container.

**Kelebihan Menggunakan Container :**
1. Isolasi lingkungan terdapat pada tingkat aplikasi / service, sehingga deployment akan lebih fleksibel per-service.
2. Pemeliharaan sistem dapat lebih fokus per-service, sehingga ketika ada update pada salah satu service dengan versi yang lebih baru tidak akan mempengaruhi service yang lain.
3. Dapat dengan mudah di scale aplikasi sehingga lebih stable ketika ada salah satu aplikasi yang mati.

Berikut beberapa Tools yang sering digunakan untuk membuat suatu **Container** :

   <img alt="image1" src={useBaseUrl('img/docs/image-11.png')} height="170px"/>
