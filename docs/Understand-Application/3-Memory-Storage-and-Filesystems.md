---
sidebar_position: 3
---

# 3. Memory and Storage

import useBaseUrl from '@docusaurus/useBaseUrl';

### MEMORY
**Memory (RAM) Random Access Memory** adalah media penyimpanan sementara. Pada sistem operasi linux, memiliki swap sebagai tambahan cadangan memory jika memory utama telah penuh. 

Untuk memeriksa penggunaan memory, jalankan perintah berikut :
```shell
sudo apt install htop -y
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/mem1.png')} height="400px"/>
  </center>

keterangan : perintah untuk melakukan instalasi htop

```shell
htop
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/mem2.png')} height="400px"/>
  </center>

keterangan : perintah untuk menjalankan htop

- **CPU** adalah berapa jumlah core yang kita miliki.
- **Mem** adalah total penggunaan memory.
- **Swp** adalah Memory cadangan.
- **Tasks** adalah aplikasi yang sedang berjalan di server.
- **Load average** adalah rata-rata aplikasi yang berjalan.
- **Uptime** adalah berapa lama server kita hidup.
- **PID** adalah nomor proses id setiap proses yang berjalan di linux.
- **VIRT** adalah memory yang terpakai.
- **Command** adalah perintah apa yang sedang di jalankan.

### Storage
**Storage** adalah sebuah media penyimpanan, pada dasarnya semua sistem operasi di install itu di atas storage.

Untuk melihat penggunaan dari **storage** kalian bisa menggunakan perintah dibawah ini.

```shell
df -h
```

  <center>
  <img alt="image1" src={useBaseUrl('img/docs/mem3.png')} height="400px"/>
  </center>

### File Systems
**File Systems** adalah pengaturan penyimpanan data yang sangat mempermudah pekerjaanmu sehari-hari. Karena sistem ini mengatur mulai dari penamaan sampai penempatan sebuah dokumen di dalam drive / storage.

**Jenis-jenis file system** :
- FAT32 : Cocok digunakan pada media penyimpanan kecil.
- NTFS : Digunakan untuk sistem operasi windows XP s.d windows 10
- EXT2/EXT3/EXT4 : Digunakan untuk sistem operasi Linux
- BTRFS : Digunakan untuk menangani masalah pada Linux seperti snapshots(Backup Data).
