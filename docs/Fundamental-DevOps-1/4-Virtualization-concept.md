---
sidebar_position: 4
---

# 4. Virtualization  

import useBaseUrl from '@docusaurus/useBaseUrl';

**Virtualization** adalah suatu teknologi yang memungkinkan kita untuk membagi sebuah resource menjadi lebih kecil dari perangkat yang memiliki resource yang besar. 
Secara sederhananya yaitu kita dapat menjalankan beberapa sistem operasi secara bersamaan.

Kemudian hal yang perlu diketahui dari virtualization adalah **Hypervisor**. 
Jadi **Hypervisor** adalah program untuk membuat dan menjalankan virtual machine.

**Virtual Machine** adalah sistem komputer yang berjalan di atas sistem lain, serta memiliki akses ke beberapa sumber daya yang ada di bawahnya. Seperti CPU, Memory dan Storage. Selain itu dapat mengakses USB, Network Card dan sebagainya.

**Berikut adalah Gambaran bagaimana Virtualization bekerja:**
<img alt="image1" src={useBaseUrl('img/docs/image-8.png')} height="280px"/>

Jadi ibaratkan di infrastructure ini kalian mempunyai resource yang besar, katakanlah kalian mempunyai CPU 30 core dan Memory 64.Gb. nah lalu kalian butuh nih untuk dipecah menjadi lebih kecil nah maka disitulah kita perlu install yang namanya virtualisasi atau dibawahnya itu adalah hypervisor. Jadi intinya Infra kita yang tadi besar itu kita pecah-pecah menjadi lebih kecil dengan menggunakan virtualisasi. contoh Jadi kalian pecah nih resource kalian yang tadi sebesar 30 core 64.Gb memory itu menjadi beberapa virtualisasi berjumlah 30 dengan spek katakanlah 1 Core 1 Memory.   

**Kelebihan menggunakan virtualization :**
1. Kemudahan backup dan recovery server-server yang dijalankan di dalam sebuah virtual machine, karena akan melakukan backup secara keseluruhan termasuk konfigurasi sistem.
2. Kemudahan deployment karena dapat di clone sebanyak mungkin dengan konfigurasi sistem yang sama.
3. Dapat memindahkan virtual machine ke server lain jika terjadi kerusakan hardware.

Berikut beberapa Platform yang sering digunakan untuk membuat suatu **Virtual Machine** :
  <img alt="image1" src={useBaseUrl('img/docs/image-9.png')} height="180px"/>
