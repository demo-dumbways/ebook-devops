---
sidebar_position: 4
---

# 4. SSH key for Github

import useBaseUrl from '@docusaurus/useBaseUrl';

**SSH key** berguna untuk mengkoneksikan local anda dengan platform github. Lalu mungkin kalian bertanya bagaimana cara untuk mendapatkan **SSH key**, serta bagaimana cara untuk mengkoneksikan local kita dengan platform github. Untuk cara ikuti step by step di bawah ini.

### 1. Generate SSH key
Untuk mendapatkan **SSH key** kalian dapat menggunakan perintah dibawah ini. 

```shell
ssh-keygen
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git3.png')} height="400px"/>
</center>

### 2. SSH key Location
Jika kalian sudah menjalankan perintah sebelumnya maka kalian sudah berhasil untuk men-generate **SSH key** yang akan kalian gunakannya. Untuk lokasi **SSH key** yang sudah kalian generate tadi berada di `.ssh/id_rsa.pub`. Jika sudah lakukan copy pada **SSH-key** tersebut.

```shell
cat .ssh/id_rsa.pub
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git4.png')} height="400px"/>
</center>

### 3. Add new SSH to github settings
Tahap selanjutnya setelah kalian melakukan copy **SSH-key** adalah memasukkannya kedalam config github dengan membuka https://github.com/settings/keys.

Jika sudah langsung tekan saja di bagian **New SSH key**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/git5.png')} height="400px"/>
</center>


Setelah itu masukkan saja **SSH key** yang sudah kalian copy tadi kebagian **key**. Jika sudah Langsung saja save dengan menge-klik bagian **Add SSH key**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/git6.png')} height="400px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/git7.png')} height="400px"/>
</center>

### 4. Check Connection
Jika kalian sudah melakukan semua step di atas maka kalian sudah berhasil meng-koneksikan local kalian dengan Github.

Untuk make sure apakah sudah terkoneksi kita bisa menggunakan perintah di bawah ini.

```shell
ssh -T git@github.com
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git8.png')} height="400px"/>
</center>

Jika muncul teks seperti ini `Hi demo-dumbways! You've successfully authenticated, but GitHub does not provide shell access.` maka kalian sudah berhasil mengkoneksikan local kalian dengan Github.