# Indihome Router Utility (Maintenance)

> **Peringatan:** :red_circle: Alat ini dibuat khusus untuk keperluan pendidikan dan penelitian. Penulis tidak bertanggung jawab atas segala bentuk penyalahgunaan atau kerusakan yang mungkin timbul dari penggunaan skrip ini. Harap gunakan dengan bijak dan hanya di lingkungan di mana Anda memiliki izin eksplisit.

Indihome Router Utility adalah alat Decoder dan Encoder config pada router seperti zte, huawei, tp-link, d-link, tenda, fiberhome dll dan alat ini baru disempurnakan untuk router zte, dengan alat ini Anda tidak perlu bersusah payah untuk mencari seputar isi konfigurasi pada router Indihome di rumah Anda.

#
Fitur yang ada pada Aplikasi Indihome Router Utility.exe 
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
- Mac Address Generator
- Hash Type Identifier
- MD5 Password Generator
- HTTP Header Checker
- Compare Text Utility

#
<b>Panduan Cara Penggunaan:</b>
1. Pastikan sebelumnya sudah menginstal "Indihome Decoder Utility" yang pernah dibahas disini https://github.com/MichaelJorky/Indihome-Decoder-Encoder-Utility
2. Download "Indihome Router Utility" caranya arahkan cursor pada bagian "code" pada "local" pilih "download zip".
3. Lalu ekstrak filenya kemudian copy isi file yang ada didalam folder "Indihome-Router-Utility-main" lalu pastekan pada folder ```.indihome-utility``` (point 1).
4. Untuk default script decodingnya maupun encodingnya menggunakan script seperti yang sudah dibahas pada (point 1) atau seperti yang tercantum dibawah ini:

<b>Default Decoder List (12 List):</b>
```
decoder.py config/config.bin config/config.xml
decoder.py --model "F670L" config/config.bin config/config.xml
decoder.py --serial ZTE123456789 config/config.bin config/config.xml
decoder.py --mac AA:BB:CC:DD:EE:FF --serial ZTE123456789 config/config.bin config/config.xml
```
<b>Default Encoder List (6 List):</b>
```
encoder.py --key 'isi_key' --signature 'F670L' --include-header config/config.xml config/new.config.bin
encoder.py --key 'isi_key' --signature 'F670L' --version 1 --include-header config/config.xml config/new.config.bin
encoder.py --signature F670L --payload-type 6 config/config.xml config/new.config.bin 
encoder.py --model "F670L" config/config.xml config/new.config.bin
encoder.py --serial ZTE123456789 --signature 'F670L' config/config.xml config/new.config.bin
encoder.py --signature 'F670L' --use-signature-encryption config/config.xml config/new.config.bin
```
5. Untuk decoding support penggunaan perintah seperti contoh yang tercantum dibawah ini:
```
--key 2bf3525fd2dcc7fe
--model F670L
--serial ZTE123456789
--mac AA:BB:CC:DD:EE:FF
--longpass Telkomdso123
--signature ZXHN F670L V9.0
--key-prefix CEFD0000000000174654
--iv-prefix ZTE%FN$GponNJ025
--key-suffix 574ffbb30a488a9e2d583a86719400a7
--iv-suffix dedb7b84041d5f10bfe84bca2a165e39
--try-all-known-keys
```
6. Untuk Encoding support penggunaan perintah seperti contoh yang tercantum dibawah ini:
```
--key 2bf3525fd2dcc7fe
--model F670L
--serial ZTE123456789
--mac AA:BB:CC:DD:EE:FF
--longpass Telkomdso123
--signature ZXHN F670L V9.0
--iv {iv_key}
--use-signature-encryption
--chunk-size 65536
--payload-type {0/1/2/3/4/5/6}
--version {1/2}
--include-header
--little-endian-header
--include-unencrypted-length
--key-prefix CEFD0000000000174654
--iv-prefix ZTE%FN$GponNJ025
--key-suffix 574ffbb30a488a9e2d583a86719400a7
--iv-suffix dedb7b84041d5f10bfe84bca2a165e39
```

