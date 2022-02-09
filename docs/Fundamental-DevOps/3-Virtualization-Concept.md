---
sidebar_position: 3
---

# 3. Virtualization  

import useBaseUrl from '@docusaurus/useBaseUrl';

**Virtualization** adalah teknologi yang dapat membagi resource besar menjadi menjadi lebih kecil. Secara sederhana kita dapat menjalankan beberapa sistem operasi secara bersamaan. Di dalam virtualization terdapat **Hypervisor** yaitu suatu program untuk membuat dan menjalankan virtual machine.


**Virtual Machine** adalah sistem operasi komputer yang berjalan di atas sistem lain, dan memiliki akses ke sumber daya yang ada di bawahnya, seperti CPU, memory, storage dan sebagainya.

## Kenapa Harus Virtualization ?

Kelebihan menggunakan virtualization :
1. Kemudahan backup dan recovery server yang dijalankan di dalam sebuah virtual machine, karena akan melakukan backup secara keseluruhan termasuk konfigurasi sistem.
2. Kemudahan deployment karena dapat di clone sebanyak mungkin dengan konfigurasi sistem yang sama.
3. Dapat memindahkan virtual machine ke server lain jika terjadi kerusakan hardware.

<center>
<img alt="image1" src={useBaseUrl('img/docs/image-8.png')} height="280px"/>
</center>

Diibaratkan, infrastructure ini memiliki sumber daya yang besar, misal spesifikasinya CPU 30 Core dan Memory 64 Gb. Kemudian Kita memiliki kebutuhan server dengan spesifikasi yang lebih kecil, maka kita dapat menggunakan virtualization untuk memecah server tersebut menjadi beberapa server yang memiliki spesifikasi lebih kecil.

## Contoh Penggunaan Virtualization

Berikut ini adalah beberapa contoh penggunaan virtualization:
1. Provider Hosting
2. Provider VPS

## Virtual Machine Platform 

<center>
  <img alt="image1" src={useBaseUrl('img/docs/image-9.png')} height="180px"/>
</center>