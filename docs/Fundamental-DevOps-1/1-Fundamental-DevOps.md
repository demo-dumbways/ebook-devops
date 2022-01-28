---
sidebar_position: 1
---

# 1. Fundamental DevOps 
import useBaseUrl from '@docusaurus/useBaseUrl';

**DevOps** adalah Kombinasi dari **DEVELOPMENT** dan **OPERATION** yang bertugas sebagai penghubung antara divisi Development (Programmer) dan Operation(Infrastructure Server). Agar bisa beradaptasi dengan cepat terhadap pembaruan maupun perubahan suatu product dan serta menghilangkan hambatan Komunikasi antara tim Development dan Operation, sehingga pada saat Deployment nantinya akan lebih konsisten dan lancar.
<center>
<img alt="image1" src={useBaseUrl('img/docs/new.pic.jpg')} height="200px"/>
</center>

**Pekerjaan DevOps divisualisasikan sebagai proses loop tak terbatas yang terdiri dari :**

<center>
<img alt="image1" src={useBaseUrl('img/docs/image-1.png')} height="300px"/>
</center>

   1. **Plan** : proses perencanaan untuk seluruh alur kerja yang dibutuhkan sebelum tim pengembang mulai menulis kode.

   2. **Code** : Setelah rencana dibuat, tim developer dapat mulai menulis kode yang dibutuhkan untuk membuat suatu product.

   3. **Build** : Setelah tim developer selesai menulis kode yang dibutuhkan, mereka akan memasukan kode tersebut ke dalam shared code repository. Developer akan mengirimkan pull request, setelah developer yang lain akan mereview perubahan yang telah dilakukan. Jika kode tidak memiliki masalah, maka developer tersebut akan menyetujui pull request yang telah dikirim sebelumnya.

   4. **Test** : Langkah selanjutnya adalah melakukan pengujian. Jika ada masalah yang ditemukan pada fase ini, maka masalah tersebut akan dikirim kembali ke tim developer untuk diselesaikan.

   5. **Realese** : Pada tahap ini, setiap perubahan kode telah melewati serangkaian pengujian dan tim IT operations telah memastikan bahwa masalah yang merusak dan regresi sudah teratasi dengan baik.

   6. **Deploy** : Tahap selanjutnya adalah deployment. Setelah production environment dibuat dan dikonfigurasi maka versi terakhir dari pengembangan yang telah dilakukan akan diterapkan.

   7. **Operate** : Pada tahap ini aplikasi sudah bisa untuk di operasikan atau digunakan.

   8. **Monitor** : Pada tahap terakhir ini, tim IT operations akan terus bekerja keras untuk memantau infrastruktur, sistem, dan aplikasi. Hal ini dilakukan untuk memastikan bahwa produk atau aplikasi yang dikembangkan dapat berjalan dengan lancar.
