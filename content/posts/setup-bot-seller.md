---
title: "Setup Bot Seller"
date: 2023-07-08T12:50:38Z
tags:
  - bot
image:
comments: false
---
Bahan - Bahan (Wajib):
1. VPS untuk host bot (disarankan ububtu 22)
2. VPS yang sudah terinstall autoscript pototo API




Setup database
1. buat akun di deta space
2. lalu buat database dan ambil api key nya
![](https://telegra.ph/file/7bc6ad9c1d736c2687487.jpg)
![](https://telegra.ph/file/79efa9a9c0c10efca9cfa.jpg)
![](https://telegra.ph/file/8f408e994cba3b3eb2b84.jpg)
![](https://telegra.ph/file/c642d47aa44e5a0f9ccc7.jpg)


Cara install:
1. upload file zip yang di berikanan oleh @madewgn ke VPS yang akan kamu gunakan untuk hosting bot nya
2. Insta keperluan bot
```bash
apt install python3 python3-pip zip unzip -y
```
3. ekstrak file zip yang di berikan 
```bash
unzip namafile.zip
```
ganti `namafile.zip` dengan nama dari file zip mu

4. install requirements 
```bash
pip3 install -r req.txt
```

5. ganti token dan menambahkan server

untuk token bot ada di file .env
ganti saja `BOT_TOKEN` dengan token bot mu dan ganti juga api key di file `plugins/config.py`
untuk nambah server baru silakan tulis di bagian `create` di file plugins/main.py
!["create"](https://telegra.ph/file/60743abc47fe3f6fb32d6.jpg)

untuk trial nya silakan di edit di file plugins/trial.py
edit yang di var `l`, kode callback yang digunakan adalah setelah spasi
misal nama servet nya `SG DO` atau `ID IKD` nah yang di ambil itu hanya `DO` dan `IKD` nya saja, itupun sudah di tambahkan `t` di awal callback nya untuk menandai bahwa itu trial, `t` untuk `trial`
!["trial"](https://telegra.ph/file/00a1806e984fc3ff6b207.jpg)

dan juga ganti domain nya dengan domain mu, serta `server1` itu var yang di ambil dati file `config.py`
!["trial2"](https://telegra.ph/file/b06d8c26bcd6519da3819.jpg)

sesuaikan juga yang di callback.py dengan yg ada dk main.py
![setup](https://telegra.ph/file/97ac9f47bfca98368a202.jpg)

6. setelah bot selesai di setup tinggal di run aja
jangan lupa pakai screen agar bot tetep hidup
```bash
screen -r bot
```
lalu jalankan dengan perintah
```bash
python3 bot.py
```



## Setup Userbot
userbot ini akan digunakan untuk mengatur saldo pada akun

1. upload file zip userbot yg telah saya berikan dan di ekstark
2. jalankan userbot nya
```bash
python3 bot.py
```

nah sekarang masukkan no tele yang kamu pakai, lalu masukkan juga kode otp yang di berikan oleh telegram

untuk tes userbot, ketik saja .ping
