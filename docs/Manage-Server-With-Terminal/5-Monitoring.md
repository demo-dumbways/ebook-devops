---
sidebar_position: 5
---

# 5. Monitoring

import useBaseUrl from '@docusaurus/useBaseUrl';

**Monitoring** merupakan aktivitas untuk melihat kinerja sistem secara realtime. Berikut ini adalah beberapa perintah yang dapat kita gunakan untuk memonitoring sebuah server.

- htop
- lsof
- ps

## Kenapa perlu Monitoring ?
- Untuk mengetahui apakah ada server down atau tidak.
- Untuk mengetahui resource dari server tersebut apakah penuh atau tidak.
- Untuk mengetahui tentang aplikasi yang berada di server kita itu jalan atau tidak, ataupun sudah up to date atau belum.

### Monitoring htop
**Htop** merupakan perintah untuk memonitoring sistem, kita dapat melihat penggunaan memory, cpu, swap. Berikut adalah contoh penggunaan :

```shell
htop
```

Jika pada server kalian belum terinstall, maka dapat menjalankan perintah beriku:

```shell
sudo apt install htop -y
```
```shell
htop
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/htop.png')} height="400px"/>
</center>

Keterangan :

- **CPU** adalah berapa jumlah core yang kita miliki.
- **Mem** adalah total penggunaan memory.
- **Swp** adalah Memory cadangan.
- **Tasks** adalah aplikasi yang sedang berjalan di server.
- **Load average** adalah rata-rata aplikasi yang berjalan.
- **Uptime** adalah berapa lama server kita hidup.
- **PID** adalah nomor proses id setiap proses yang berjalan di linux.
- **VIRT** adalah memory yang terpakai.
- **Command** adalah perintah apa yang sedang di jalankan.

## Monitoring nmon
Pada tampilan awal terdapat beberapa pilihan yang dapat kita gunakan, berikut hanyalah contoh penggunaannya :

Untuk instalasi nmon dapat menggunakan perintah berikut :
```shell
sudo apt install nmon
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/nmon.png')} height="400px"/>
</center>

Untuk menjalankan nmon kalian dapat menggunakan perintah dibawah ini
```shell
nmon
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/nmon2.png')} height="400px"/>
</center>

Keterangan : 
Disini kita dapat memilih ingin memonitoring apa saja, Disini kita coba saja untuk menampilkan beberapa saja.

- **c** adalah CPU
- **m** adalah Memory
- **d** adalah Disk
- **n** adalah network

Berikut adalah tampilan dari nmon untuk menampilkan **cpu, memory, disk, dan network**

<center>
<img alt="image1" src={useBaseUrl('img/docs/nmon3.png')} height="400px"/>
</center>

## Monitoring lsof
Lsof merupakan singkatan list open files, berfungsi untuk melihat seluruh file yang terbuka berdasarkan proses aktif yang berjalan di sistem. 

Berikut adalah contoh penggunaan :
```shell
lsof
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/lsof1.png')} height="400px"/>
</center>

keterangan : untuk menampilkan seluruh proses

```shell
lsof -u (your-user)
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/lsof2.png')} height="400px"/>
</center>

keterangan : menampilkan proses yang dilakukan oleh user “your-user”

```shell
lsof -i :80
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/lsof3.png')} height="400px"/>
</center>

keterangan : untuk menampilkan proses yang menggunakan port 80

## Monitoring ps
Ps merupakan singkatan dari process status, untuk mengetahui daftar proses yang berjalan pada sistem. 

Berikut adalah contoh penggunaan :
```shell
ps -f -u (your-user)
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ps1.png')} height="400px"/>
</center>

keterangan : untuk menampilkan proses pada user “your-user”

```shell
ps -aux
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/ps2.png')} height="400px"/>
</center>

keterangan : untuk menampilkan seluruh proses secara lengkap