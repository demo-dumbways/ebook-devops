---
sidebar_position: 5
---

# 5. Install Ubuntu Server

import useBaseUrl from '@docusaurus/useBaseUrl';

## Requirements

Sebelum melakukan instalasi ubuntu server, hal pertama yang harus kita lakukan adalah menginstall tools virtual machine serta meng-unduh file ISO server terlebih dahulu.Pada materi kali ini, kita akan menggunakan tools **VMware Workstation Player**.

Silahkan klik link dibawah untuk meng-unduh tools yang diperlukan.

- **VMware Installation     : [Download](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html)**
- **Ubuntu Server 20.04     : [Download](https://ubuntu.com/download/server)**

### 1. Installation Ubuntu Server

1. Buka Virtual machine kalian, untuk contohnya disini menggunakan VMware. Jika sudah langsung klik saja di bagian **Create a new Virtual Machine**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm1.png')} height="350px"/>
</center>

2. Jika sudah nanti akan masuk ke halaman seperti gambar dibawah. Disini kalian pilih saja di bagian **use ISO image**. Setelah itu masuk ke bagian **browser** lalu cari lokasi **ISO ubuntu server** yang sudah kalian download sebelumnya.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm2.png')} height="380px"/>
</center>

3. Lalu tahapan selanjutnya masukan saja user dan password yang kalian inginkan.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm3.png')} height="380px"/>
</center>

4. Tahapan selanjutnya adalah menentukan lokasi dimana Virtual machine kalian ingin disimpan.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm4.png')} height="380px"/>
</center>

5. Setelah atur size disk yang ingin kalian gunakan. Disini sebagai contoh saya menggunakan 10GB. Disini ada 2 pilihan yaitu **Store Disk as a single file** dan **Split virtual disk into multiple files**. 

   Keterangan :
     - **Store Disk as a single file** maksudnya adalah disk yang kalian buat itu nantinya akan langsung terbuat 10Gb. (ini tidak disarankan untuk pengguna yang memiliki hardisk yang berkapasitas kecil).
     - **Split virtual disk into multiple files** maksudnya adalah disk yang kita pakai untuk virtual machine kita nantinya itu akan dibagi menjadi beberapa bagian. Jadi walaupun kita menggunakan disk berkapasitas 10Gb itu nanti tidak akan terpakai seluruhnya.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm5.png')} height="380px"/>
</center>

6. Sekarang kita akan meng-customisasi hardware untuk server kita, tekan saja di bagian **Customize Hardware**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm6.png')} height="380px"/>
</center>

7. Disini ada beberapa pilihan untuk kita melakukan customisasi seperti **Memory**, **Processors** dan **Network adapter**. 

   Keterangan:
     - **Memory** berfungsi untuk penyimpanan data yang ingin kita gunakan untuk Virtual Machine yang ingin kita buat. Disini kita pilih gunakan saja defaultnya yaitu sebesar 4Gb tetapi misalkan kalian merasa kurang kalian boleh untuk menaikkannya sesuai keinginan kalian.
     - **Processors** adalah salah satu komponen penting untuk Virtual Machine yang ingin kita bangun, serta berfungsi untuk memproses data dan mengontrol sistem yang ada pada Virtual Machine kita. Disini kita menggunakan defaultnya saja yaitu sebesar 2 core.
     - **Network adapter** berfungsi untuk menghubungkan komputer ke jaringan. Untuk penjelasan lebih lanjut ada di poin berikutnya.

8. Jika sudah selesai untuk meng-setting **memory** dan **processor**, kalian bisa pergi ke bagian **Network Adapter**. Setelah itu ubah dari defaultnya yaitu **NAT** menjadi **Bridge**.

   Keterangan:
     - kalau menggunakan **NAT** nantinya server yang kita buat ini akan mendapatkan IP yang sudah di sediakan oleh Virtual Machine kita.
     - Kalau Menggunakan **Bridge** nantinya server yang kita buat akan mendapatkan IP dari internet yang sedang kita gunakan.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm7.png')} height="380px"/>
</center>

9. Jika sudah langsung klik saja **Close**.

10. Setelah nanti kalian akan di kembalikan ke halamannya sebelumnya, setelah itu tekan saja di bagian **Finish**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm8.png')} height="450px"/>
</center>

11. Jika sudah nantinya kalian akan langsung di arahkan ke bagian installasi, disini kalian tunggu saja sampai prosesnya selesai.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm9.png')} height="430px"/>
</center>

12. Jika sudah kalian akan muncul tampilan seperti gambar dibawah ini. Setelah itu pilih bahasa yang ingin digunakan **English**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm10.png')} height="300px"/>
</center>

13. Proses ini bisa langsung kalian skip dengan klik **Done**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm11.png')} height="300px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm12.png')} height="300px"/>
</center>

14. Selanjutnya kita akan ubah konfigurasinya dari yang awalnya itu **DHCPv4** menjadi **Static**.

    Keterangan:
      - **DHCP (Dynamic Host Protocol Configuration)** : Alamat IP yang dapat berubah-ubah pada perangkat yang tersambung setiap kali terhubung kembali pada jaringan tersebut (otomatis).
      - **Static** : Alamat IP tidak berubah-ubah dari yang telah diberikan oleh adminisitrator (setting manual)

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm13.png')} height="300px"/>
</center>

15. Pilih di bagian **ens33**, setelah itu pada bagia **IPv4 Method** ubah dari yang awalnya **automatic** menjadi **manual**. Setelah itu masukan detail IP pada form yang tersedia(kalian bisa masukkan saja IP yang sudah tertera di bagian DHCPv4). Jika sudah langsung tekan saja **Save**.

     Keterangan:
       - **Subnet**       : Istilah teknologi Informasi yang membedakan Network ID dan Host ID atau sebagai penentu porsi Network ID dan Host ID pada deretan kode biner
       - **Address**      : Alamat **IP** yang akan digunakan untuk Virtual Machine yang akan  kalian buat. (kalian dapat mengisi bagian ini dengan IP yang sudah ada di bagian DHCP)
       - **Gateway**      : Perangkat komputer yang berfungsi untuk mengkoneksikan sebuah Jaringan komputer terhadap satu jaringan komputer yang lain.
       - **Name servers** : Dibagian **Name servers** ini kalian cukup memasukkan IP DNS dari google supaya dapat terhubung dengan browser.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm14.png')} height="300px"/>
</center>

16. Jika konfigurasi sudah selesai maka akan ada perubahan di bagian **DHCPv4** tadi menjadi **static**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm15.png')} height="300px"/>
</center>

17. Pada tahap selanjutnya kalian bisa skip dengan klik **Done**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm16.png')} height="300px"/>
</center>

18. Pada tahap selanjutnya kalian bisa skip lagi dengan klik **Done**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm17.png')} height="300px"/>
</center>

19. Disini kita dapat memilih bagian **Custom storage layout**. Kenapa kita memilih **Custom storage layout** karena kita akan membuat 2 buah partisi, jika sudah kalian pilih setelah itu langsung saja klik **Done**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm18.png')} height="300px"/>
</center>

20. Selanjutnya disini kita akan membuat 2 buah partisi untuk **root** dan **swap**. Langsung pilih saja di bagian **/dev/sda** lalu pilih di bagian **Add GPT Partition**. Untuk kapasitasnya kalian bisa samakan saja dengan gambar dibawah (kecuali untuk swap, kalian bisa setting semau kalian apabila merasa kurang).

    Keterangan :
      - **root** adalah tempat dimana sistem kita itu ter-install.
      - **swap** adalah suatu memory cadangan yang akan digunakan untuk server kita apabila memory utama sudah penuh.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm19.png')} height="300px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm20.png')} height="300px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm21.png')} height="300px"/>
</center>

21. Jika sudah disini kita sudah berhasil membuat 2 partisi untuk **root** dan **swap**. Jika sudah langsung saja klik **Done**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm22.png')} height="300px"/>
</center>

22. Lalu akan muncul notifikasi untuk mengkonfirmasi semua konfigurasi yang sudah kita buat. Jika sudah langsung klik saja **Continue**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm23.png')} height="300px"/>
</center>

23. Selanjutnya masukan informasi seperti nama, username, dan password untuk server yang kalian buat. Jika sudah klik saja **Done**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm24.png')} height="390px"/>
</center>

24. Ditahapan ini jangan lupa untuk checklist bagian **Install OpenSSH server** gunanya adalah untuk me-remote server yang kita buat.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm25.png')} height="310px"/>
</center>

25. Pada tahap selanjutnya skip dengan klik **Done**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm26.png')} height="300px"/>
</center>

26. Kita sudah selesai untuk tahapan instalasinya. Tunggu saja proses instalasi sampai selesai jika sudah selesai langsung saja klik **Reboot Now**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm27.png')} height="300px"/>
</center>

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm+.png')} height="295px"/>
</center>

27. Jika tahapan installasi sudah selesai. Masukkan **id** beserta **password** yang sudah kalian set-up sebelumnya, Jika sudah maka kalian telah berhasil melakukan instalasi ubuntu server.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm28.png')} height="400px"/>
</center>

28. Untuk make sure apakah server yang kalian buat ini sudah terhubung ke dalam internet bisa gunakan perintah dibawah ini

 ```shell
 ping google.com
 ```

- Jika server kalian sudah terhubung ke dalam internet maka akan muncul seperti gambar dibawah ini.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm-.png')} height="150px"/>
</center>

29. Jika kalian ingin melakukan customisasi untuk **IP** dari server yang sudah kalian buat kalian bisa gunakan perintah berikut

```shell
sudo nano /etc/netplan/00-installer-config.yaml
```

30. Jika kalian sudah menggunakan perintah di atas maka akan muncul Teks editor seperti gambar dibawah ini. Selanjut di bagian **addresses** kalian bisa ubah dengan IP yang kalian inginkan. Lalu untuk keluar dari teks editor ini kalian bisa menggunakan **ctrl + x** lalu **Y** setelah itu **Enter**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/custom1.png')} height="400px"/>
</center>

31. Selanjutnya untuk mengkonfirmasi customisasi **IP** yang sudah kalian buat tadi kalian bisa menggunakan perintah dibawah.

```shell
sudo netplan apply
```

32. Jika sudah maka kita coba cek apakah sudah terhubung dengan internet atau tidak bisa menggunakan perintah dibawah.

```shell
ping google.com
```

33. Jika sudah terhubung dengan internet maka akan muncul notifikasi seperti gambar di bawah ini.

<center>
<img alt="image1" src={useBaseUrl('img/docs/custom2.png')} height="400px"/>
</center>


### 2. Remote Server

1. Untuk me-remote server kalian bisa gunakan perintah seperti ini
   ```shell
   ssh alvin@192.168.1.6
   ```
   Pastikan dibagian user(alvin), dan IP(192.168.1.6) ubah dengan user dan IP server yang sudah kalian buat sebelumnya. Jika sudah nanti akan muncul **Are you sure you want to continue connecting** langsung ketik saja **yes**. Jika sudah masukkan Password dari Server yang sudah kalian buat sebelumnya.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm29.png')} height="300px"/>
</center>

2. Selanjutnya tahapan pertama yang harus kita lakukan pada saat sedang berada di dalam server yaitu melakukan update serta upgrade terlebih dahulu gunanya untuk menjaga agar system kita tetap up-to-date.

  Untuk melakukan update dan upgrade, kalian bisa menggunakan perintah di bawah ini.

  ```shell
  sudo apt update; sudo apt upgrade
  ```

3. selanjutnya kita akan coba untuk menginstall aplikasi **Nginx**.
  
  Kalian bisa gunakan perintah di bawah ini.  
  ```shell
  sudo apt install nginx
  ```

  Lalu nanti akan muncul notifikasi **Do you want to continue? [Y/n]** kalian ketik saja **Y**. Jika sudah maka instalasi akan berjalan.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm30.png')} height="350px"/>
</center>

4. Jika instalasi sudah selesai kita bisa cek dengan menggunakan perintah dibawah ini.

  ```shell
  sudo systemctl status nginx
  ```

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm31.png')} height="350px"/>
</center>

5. Sekarang coba buka browser kalian, lalu masukkan **IP dari server kalian**.

<center>
<img alt="image1" src={useBaseUrl('img/docs/vm32.png')} height="350px"/>
</center>
