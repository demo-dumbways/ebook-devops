---
sidebar_position: 4
---

# 4. Git Config

import useBaseUrl from '@docusaurus/useBaseUrl';

:::info
Sebelumnya Pastikan kalian sudah memiliki akun **github**.
:::

Hal pertama yang harus kalian lakukan adalah menetapkan nama **pengguna** dan alamat **email**, untuk perintahnya kalian dapat menggunakan perintah dibawah ini. 

:::warningAttention
Pastikan **user.name** dan **user.email** sesuai dengan **github** akun kalian.
:::

```shell
git config --global user.name "your.github-user.name"
```

```shelll
git config --global user.email "your.github-user.email"
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/git1.png')} height="400px"/>
</center>

Jika kalian sudah menjalankan perintah di atas, kalian bisa cek **user.name** dan **user.email** kalian sudah tepat atau belum dengan menggunakan perintah dibawah ini.

```shell
git config --list
```
<center>
<img alt="image1" src={useBaseUrl('img/docs/git2.png')} height="400px"/>
</center>