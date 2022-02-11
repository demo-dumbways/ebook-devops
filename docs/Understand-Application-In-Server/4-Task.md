---
sidebar_position: 4
---

# 4. Task

import useBaseUrl from '@docusaurus/useBaseUrl';

## 4.1 Instruksi

:::caution
Pastikan untuk melakukan screenshot step by step yang dilakukan, untuk digunakan sebagai dokumentasi tugas.
:::

Setelah mempelajari terkait konfigurasi dan instalasi linux server, maka silakan buat sebuah environment linux dengan ketentuan sebagai berikut:

<center>
<img alt="image1" src={useBaseUrl('img/docs/task.png')} />
</center>

### VMware Environment
- Disk       : 10 Gb
- Memory     : 2 Gb
- Processors : 2 Cores
- Network    : NAT

### Ubuntu Settings
- Bahasa       : English
- Network      : Static
- Storage      : Custom Storage Layout
- Username     : (your-user-name)
- Password     : (your-password)
- Server Name  : (your-name)
- OpenSSH      : True

### Setelah Linux Terinstall
- Application  : Install Apache2 Secara Manual
- Apache dapat diakses melalui browser

## 4.2 Pengumpulan
1. Pastikan untuk clone repository berikut ini, sebagai template tugas: https://github.com/dumbwaysdev/dumbways-report
2. Tulis step-by-step yang telah Anda lakukan secara detail dan sertakan screenshot setiap prosesnya. 
3. Setelah menyelesaikan tugas, silakan push pekerjaan Anda ke repository milik Anda. 
4. Upload tugas yang telah dibuat ke repository GitHub Anda.

Referensi:
- [Version Control](/Getting-Started/Version-control/Git-Installation)

## 4.3 Project Management
Tambahkan deskripsi berikut ke dalam kanban pada project management Anda
```
Konfigurasi environment dan instalasi linux server, dimana server tersebut dapat terkoneksi ke internet dan juga dapat di akses melalui SSH / Browser.

- [ ] Definisikan apa itu DevOps menurut pemahamanmu
- [ ] Buatlah environment untuk server (CPU, Memory, Storage dan Network)
- [ ] Install linux ubuntu server 18.x / 20.x dengan VMware
- [ ] Gunakan IP static untuk linux ubuntu server
- [ ] Buat swap memory and root partition
- [ ] Docker terinstal secara otomatis setelah proses instalasi linux ubuntu server
- [ ] Local server dapat terkoneksi dengan internet
- [ ] Dapat di SSH dari lokal komputer ke dalam virtual machine
- [ ] Instalasi apache2 secara manual dan dapat di akses melalui browser
```

Referensi:
- [Membuat GitHub Project](/Getting-Started/Project-Management/Make-Project-Management)
- [Manage GitHub Issue](/Getting-Started/Project-Management/Issue-Dan-Status-Project)

## 4.4 Diskusi
Silakan diskusikan terkait kendala atau kesulitan selama pembelajaran pada platform diskusi (slack/talk.ink) dengan membuat thread, misalnya "Introduction DevOps: problem cannot connect to network in VMware" 