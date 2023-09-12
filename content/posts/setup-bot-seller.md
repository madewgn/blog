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
apt install unzip -y
```
3. ekstrak file zip yang di berikan 
```bash
unzip namafile.zip
```
ganti `namafile.zip` dengan nama dari file zip mu

4. install bahan²
```bash
cd <hasil-unzip>
```
```bash
./install.sh
```

5. ganti token dan menambahkan server

untuk token bot ada di file .env
ganti saja `BOT_TOKEN` dengan token bot mu dan ganti juga api key di file `plugins/config.py`
untuk menambahkan server baru cukup gunakan cmd `/add` di bot telegram
!["create"](https://telegra.ph/file/60743abc47fe3f6fb32d6.jpg)

6. setelah bot selesai di setup tinggal di run aja
jangan lupa pakai screen agar bot tetep hidup
```bash
screen -S bot
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
