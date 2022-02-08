---
sidebar_position: 10
---

# 10. Git Branch

import useBaseUrl from '@docusaurus/useBaseUrl';

**Git branch** merupakan perintah yang dibuat untuk membuat versi dari sebuah repository. Seperti kita melakukan clone terhadap sebuah folder dimana folder lainnya dapat diubah atau dihapus lebih leluasa.

Penggunaan di lapangan, git branch digunakan untuk membuat versi :
- Development
- Staging
- Production

## Make Branch :
Untuk membuat branch kalian bisa menggunakan beberapa perintah berikut

### 1. git branch 

```shell
git branch (name branch)
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git26.png')} height="400px"/>
</center>

keterangan : membuat branch dengan nama development
### 2. git checkout

```shell
git checkout (name branch)
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git27.png')} height="400px"/>
</center>

keterangan : untuk berpindah branch
### 3. git branch -m

```shell
git branch -m (name branch)
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git28.png')} height="400px"/>
</center>

keterangan : untuk membuat branch baru serta pindah kedalam branch tersebut
### 4. git branch -a

```shell
git branch -a
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git29.png')} height="400px"/>
</center>

keterangan : untuk melihat list branch yang dimiliki