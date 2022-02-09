---
sidebar_position: 6
---

# 6. Cloud Computing Concept

import useBaseUrl from '@docusaurus/useBaseUrl';

## 6.1 Apa itu Cloud Computing?
**Cloud Computing** merupakan sebuah teknologi yang memungkinkan kita untuk mengatur/berbagai layanan melalui internet, seperti data storage, servers, databases, networking dan software. 

## 6.2 Kenapa Harus Cloud Computing?

Bagi kebanyakan orang cloud computing sangat diminati karena beberapa alasan:
1. Dapat menghemat biaya, karena tidak perlu membeli server fisik yang harganya mahal
2. Dapat meningkatkan produktivitas, karena tidak perlu untuk setup server, jaringan dan sebagainya
3. Efektif dan efisien, karena kita tidak perlu untuk pergi keluar negeri jika ingin menambah sebuah server baru
4. Keamanan data terjamin, karena pihak cloud yang memastikan keamanannya

## 6.3 Jenis Cloud Computing

<center>
   <img alt="image1" src={useBaseUrl('img/docs/image-12.png')} height="350px"/>
</center>

### 1. Infrastructure as a Service
   
Layanan cloud yang pada dasarnya adalah suatu server fisik dan juga komputer virtual. Setiap penyedia layanan IaaS akan menyediakan resource cloud, seperti storage, jaringan, dan juga ruang data. Pada intinya kita bisa menentukan sendiri, ingin menggunakan berapa besar core, memory, storage hingga jumlah internet yang diinginkan. 

**Contohnya**
- AWS (Amazon Web Service)
- GCP (Google Cloud Platform)
- Azure (Microsoft Azure)

### 2. Platform as a Service

Layanan cloud yang disediakan dalam bentuk platform dan dapat dimanfaatkan untuk menjalankan aplikasi di atasnya. Dengan PaaS kita dapat menjalankan aplikasi tanpa harus pusing memikirkan server, network dan sebagainya. Sehingga developers dapat fokus pada pengembangan aplikasi saja.

**Contohnya**
- Heroku
- Netlify
- Dokku

### 3. Software as a Service

Layanan cloud dimana kita tinggal memakai perangkat lunak yang telah disediakan oleh pembuatnya. 

**Contohnya**
- Youtube
- Facebook
- Instagram
- TikTok

## 6.4 Tipe Cloud Computing

### 1. Private Cloud

<center>
   <img alt="image1" src={useBaseUrl('img/docs/image-13.png')} height="180px"/>
</center>

**Private Cloud** adalah layanan yang disediakan kepada orang tertentu. Biasanya hanya diterapkan dalam suatu perusahaan yang memiliki data dalam jumlah besar tetapi bersifat rahasia.

Karakteristik Private Cloud:
- Dapat di scale secara mandiri dengan pengetahuan teknis
- Management data hanya dapat diakses oleh staf IT tertentu
- Tidak perlu membayar biaya layanan jika orang menggunakannya

Contoh Private Cloud:
- Menggunakan OpenStack atau teknologi sejenis dan hanya dapat diakses melalui VPN (Virtual Private Network)
- Aplikasi yang hanya dapat di akses melalui jaringan internet local

### 2. Public Cloud

<center>
   <img alt="image1" src={useBaseUrl('img/docs/image-14.png')} height="180px"/>
</center>

**Public Cloud** adalah layanan yang disediakan kepada publik. Biasanya digunakan untuk mempublikasikan data mereka secara publik, baik itu dalam bentuk object seperti foto, video, dokumen dan sebagainya.

Karakteristik Public Cloud :
- Dapat di scale dengan mudah, tanpa pengetahuan teknis
- Ada biaya layanan yang harus dibayar setiap bulannya
- Fleksibel, karena dapat dihapus dan dapat dibuat ulang

Contoh Public Cloud:
- AWS (Amazon Web Service)
- GCP (Google Cloud Platform)
- Azure (Microsoft Azure)