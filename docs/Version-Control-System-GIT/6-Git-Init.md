---
sidebar_position: 6
---

# 6. Repository

import useBaseUrl from '@docusaurus/useBaseUrl';

Reporsitory adalah tempat untuk menampung setiap perubahan pada git. Misalkan kita memiliki sebuah directory yang menggunakan git artinya directory tersebut adalah **repository**

## Make repository
Untuk membuat repository itu ada 2 cara berikut adalah perintah untuk membuatnya.

### 1. Cara pertama
Untuk cara pertama membuat **repository** sendiri kita bisa menggunakan perintah berikut :                
 `git init (nama-repository-yang-kalian-inginkan)` 

```shell
git init dumbways
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git9.png')} height="500px"/>
</center>

### 2. Cara kedua
Untuk cara kedua kita dapat membuat **directory** terlebih dahulu, setelah itu baru melakukan **inisialisasi** untuk directory tersebut :

```shell
mkdir dumbways.id
```

```shell
cd dumbways.id
```

```shell
git init
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git10.png')} height="500px"/>
</center>