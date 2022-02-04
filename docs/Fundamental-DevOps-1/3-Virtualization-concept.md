---
sidebar_position: 3
---

# 3. Virtualization  

import useBaseUrl from '@docusaurus/useBaseUrl';

**Virtualization** adalah teknologi yang dapat membagi resource besar menjadi menjadi lebih kecil. Secara sederhana kita dapat menjalankan beberapa sistem operasi secara bersamaan. Di dalam virtualization terdapat **Hypervisor** yaitu suatu program untuk membuat dan menjalankan virtual machine.


**Virtual Machine** adalah sistem operasi komputer yang berjalan di atas sistem lain, dan memiliki akses ke sumber daya yang ada di bawahnya, seperti CPU, memory, storage dan sebagainya.

## Kenapa Virtualization ?

Kelebihan menggunakan virtualization :
- Kemudahan backup dan recovery server-server yang dijalankan di dalam sebuah virtual machine, karena akan melakukan backup secara keseluruhan termasuk konfigurasi sistem.
- Kemudahan deployment karena dapat di clone sebanyak mungkin dengan konfigurasi sistem yang sama.
- Dapat memindahkan virtual machine ke server lain jika terjadi kerusakan hardware.

**Berikut adalah Gambaran bagaimana Virtualization bekerja:**
<center>
<img alt="image1" src={useBaseUrl('img/docs/image-8.png')} height="280px"/>
</center>

Jadi ibaratkan di infrastructure ini kalian mempunyai resource yang besar, katakanlah kalian mempunyai CPU 30 core dan Memory 64 Gb. nah lalu kalian butuh nih untuk dipecah menjadi lebih kecil nah maka disitulah kita perlu install yang namanya virtualisasi atau dibawahnya itu adalah hypervisor. Jadi kalau kita menggunakan virtualisasi ini Infra kita yang sebelumnya besar tadi, itu bisa kita pecah-pecah menjadi beberapa bagian yang lebih kecil dengan menggunakan virtualisasi ini. contoh Jadi resource kalian yang sebesar 30 core 64 Gb memory tadi, Itu bisa menjadi beberapa virtualisasi berjumlah 30 dengan spek 1 Core 1 Memory. 

## Virtual Machine Platform 
<center>
  <img alt="image1" src={useBaseUrl('img/docs/image-9.png')} height="180px"/>
</center>