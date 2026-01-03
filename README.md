# Indihome / ZTE Router Utility (Maintenance)

> **Peringatan:** 🔴  
> Alat ini dibuat untuk keperluan **edukasi dan penelitian**.  
> Penulis tidak bertanggung jawab atas penyalahgunaan atau kerusakan yang timbul.  
> Gunakan hanya pada perangkat dan jaringan yang Anda miliki izin resmi.

Indihome Router Utility adalah aplikasi **GUI (Graphical User Interface)** untuk membantu proses **decode dan encode konfigurasi router**, khususnya router **OEM ZTE (Indihome, Telkomsel One, PLDT, GLOBE, MyRepublic, Biznet, MNC Play, XL Satu)**, serta berbagai utilitas jaringan pendukung.

---

## 💡 Versi Lain yang Tersedia

Project ini tersedia dalam beberapa versi sesuai kebutuhan pengguna:

- 📜 **Versi Manual / Source (CLI, Developer Mode)**  
  https://github.com/MichaelJorky/Indihome-Decoder-Encoder-Utility

- 📦 **Versi Portable (CLI, tanpa install Python)**  
  https://github.com/MichaelJorky/Indihome-ZTE-Config-Decoder-Encoder-Portable

- 🖥️ **Versi GUI (repo ini)**  
  Cocok untuk pengguna umum dan penggunaan harian

---

## ✨ Fitur Utama

Aplikasi **Indihome Router Utility.exe** menyediakan berbagai alat, antara lain:

- Decoder & Decryption Tools  
- Encoder & Encryption Tools  
- Decoder Generator  
- Encoder Generator  
- Router ADC (Auto Download Configuration)  
- Ping & Trace Route  
- Open Port Checker  
- FTP Utility  
- Telnet Utility  
- SSH Utility  
- Grab Proxy List Server  
- MAC Address Generator  
- Hash Type Identifier  
- MD5 Password Generator  
- HTTP Header Checker  
- Compare Text Utility  

> ⚠️ Saat ini fitur **Decoder & Encoder** difokuskan dan dioptimalkan untuk **router ZTE**.

---

## 📘 Panduan Penggunaan (Sementara)

### 1️⃣ Persiapan
Pastikan Anda sudah memiliki **script decoder & encoder** dari versi manual:
https://github.com/MichaelJorky/Indihome-Decoder-Encoder-Utility

### 2️⃣ Download GUI
- Klik tombol **Code**
- Pilih **Download ZIP**
- Ekstrak file

### 3️⃣ Instalasi
- Salin isi folder `Indihome-Router-Utility-main`
- Tempelkan ke folder:
```

.indihome-utility

````

### 4️⃣ Script Default yang Digunakan

#### 🔓 Default Decoder (contoh)
```bash
decoder.py config/config.bin config/config.xml
decoder.py --model "F670L" config/config.bin config/config.xml
decoder.py --serial ZTE123456789 config/config.bin config/config.xml
decoder.py --mac AA:BB:CC:DD:EE:FF --serial ZTE123456789 config/config.bin config/config.xml
````

#### 🔐 Default Encoder (contoh)

```bash
encoder.py --key 'isi_key' --signature 'F670L' --include-header config/config.xml config/new.config.bin
encoder.py --signature F670L --payload-type 6 config/config.xml config/new.config.bin 
encoder.py --model "F670L" config/config.xml config/new.config.bin
encoder.py --serial ZTE123456789 --signature 'F670L' config/config.xml config/new.config.bin
```

---

## 🔓 Opsi Decode yang Didukung

```bash
--key
--model
--serial
--mac
--longpass
--signature
--key-prefix
--iv-prefix
--key-suffix
--iv-suffix
--try-all-known-keys
```

---

## 🔐 Opsi Encode yang Didukung

```bash
--key
--model
--serial
--mac
--longpass
--signature
--iv
--use-signature-encryption
--payload-type {0/1/2/3/4/5/6}
--include-header
--little-endian-header
--include-unencrypted-length
```

---

## 🚧 Status Pengembangan

🛠️ **Maintenance / Development Mode**
Beberapa fitur masih disempurnakan.
Versi stabil direncanakan rilis dalam waktu dekat.

---

## 📌 Catatan

* Untuk fleksibilitas maksimal → gunakan **Versi Manual**
* Untuk kemudahan tanpa install → gunakan **Versi Portable**
* Untuk penggunaan visual → gunakan **Versi GUI (repo ini)**

---

## ⭐ Penutup

Jika project ini membantu:

* ⭐ Beri star
* 🐞 Laporkan bug
* 💡 Kirim saran

Terima kasih sudah menggunakan **Indihome Router Utility**.

```
