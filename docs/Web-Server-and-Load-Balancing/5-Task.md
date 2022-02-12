---
sidebar_position: 5
---

# 5. Task

import useBaseUrl from '@docusaurus/useBaseUrl';

## 5.1 Instruksi

:::caution
Pastikan untuk melakukan screenshot step by step yang dilakukan, untuk digunakan sebagai dokumentasi tugas.
:::

Setelah mempelajari terkait web server, reverse proxy dan load balancing maka buatlah konfigurasi dengan ketentuan sebagai berikut:

<center>
<img alt="image1" src={useBaseUrl('img/docs//++.png')} />
</center>

### Ketentuan
- Jalankan 1 aplikasi yang sama pada 2 buah server
- Buatlah sebuah konfigurasi reverse proxy pada server gateway (nginx)
- Buatlah sebuah konfigurasi load balancing pada server gateway (nginx)
- Aplikasi dapat di akses menggunakan domain virtual dan otomatis load balance ke 2 aplikasi tersebut

## 5.2 Pengumpulan
1. Pastikan untuk mengerjakan tugas mingguan pada medium.com.
2. Tulis step-by-step yang telah Anda lakukan secara detail dan sertakan screenshot setiap prosesnya. 
3. Setelah menyelesaikan tugas, silakan publish artikel yang sudah dibuat.

Referensi:
- [Medium](/Getting-Started/Medium/Medium)

## 5.3 Project Management
Tambahkan deskripsi berikut ke dalam kanban pada project management Anda
```
Konfigurasi web server dengan reverse proxy dan load balancing hingga dapat di akses melalui browser.

- [ ] Definisikan apa itu Web Server menurut pemahamanmu
- [ ] Buatlah 3 buah server (server gateway, server aplikasi1, server aplikasi2)
- [ ] Instal web server nginx pada server gateway
- [ ] Instal aplikasi nodejs pada server aplikasi1 dan server aplikasi2
- [ ] Buatlah sebuah konfigurasi reverse proxy pada server gateway yang mengarah ke server aplikasi1 dengan domain dumbways.xyz
- [ ] Buatlah sebuah konfigurasi load balancing pada server gateway yang mengarah ke server aplikasi2 dengan domain loadbalance.dumbways.xyz
```

Referensi:
- [Membuat GitHub Project](/Getting-Started/Project-Management/Make-Project-Management)
- [Manage GitHub Issue](/Getting-Started/Project-Management/Issue-Dan-Status-Project)

## 5.4 Diskusi
Silakan diskusikan terkait kendala atau kesulitan selama pembelajaran pada platform diskusi (slack/talk.ink) dengan membuat thread, misalnya "Introduction DevOps: problem cannot connect to network in VMware" 