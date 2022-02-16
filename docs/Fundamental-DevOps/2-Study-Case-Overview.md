---
sidebar_position: 2
---

# 2. Study Case Overview

import useBaseUrl from '@docusaurus/useBaseUrl';

Pada pembelajaran kali ini kita akan mengkonfigurasi dan menginstall linux server yang dapat digunakan untuk kebutuhan DevOps. Kita akan menggunakan ubuntu dengan beberapa konfigurasi seperti setting environment, cpu, memory, storage dan network sehingga server dapat terkoneksi ke internet.

Seperti gambar berikut:

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm28.png')} />
</center>

## 2.1 VMware Environment

- Disk : 10 Gb
- Memory : 2 Gb
- Processors : 2 Cores
- Network : Bridge

## 2.2 Ubuntu Settings

- Bahasa : English
- Network : Static
- Storage : Custom Storage Layout
- Username : (your-user-name)
- Password : (your-password)
- Server Name : (your-name)
- OpenSSH : True
