---
sidebar_position: 9
---

# 9. Git push

import useBaseUrl from '@docusaurus/useBaseUrl';

**Git push** merupakan proses upload data yang ada di database git local ke database git di server. Untuk melakukan hal tersebut kita harus melakukan perintah di bawah ini.

```shell
git push origin master
```

<center>
<img alt="image1" src={useBaseUrl('img/docs/git24.png')} height="400px"/>
</center>

**Keterangan** 
- origin adalah nama remote yang sudah kalian tambahkan tadi.
- master adalah branch default yang ada di local kita.

Jika kalian sudah melakukan perintah di atas, sekarang buka github kalian lalu lakukan refresh pada web.browser kalian. Maka file-file yang berada di local kalian sebelumnya sudah ter-upload ke dalam **Github**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/git25.png')} height="400px"/>
</center>