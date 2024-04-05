# Indihome Router Utility (iru-gui.exe)

Indihome Router Utility adalah alat Decoder dan Encoder config pada router seperti zte, huawei, tp-link, d-link, tenda, fiberhome dll dan alat ini baru disempurnakan untuk router zte, dengan alat ini Anda tidak perlu bersusah payah untuk mencari seputar isi konfigurasi pada router di rumah Anda.

![alt text](https://github.com/MichaelJorky/Indihome-Router-Utility/blob/main/img/default.jpg?raw=true)
#
Fitur yang ada pada Aplikasi Indihome Router Utility.exe 
- Decoder/Decrypt
- Encoder/Encrypt
- Decoder Generator
- Encoder Generator
- Router Login (Fake UA Android, Fake UA iOs, Fake UA, Linux, Fake UA Windows, Fake UA Ubuntu, Fake UA Debian, Fake UA Mac OS, Fake UA Chromium OS
- Ping
- Trace Route
- Port Checker
- FTP
- Telnet
- SSH
- Mac Generator
- Hash Identifier
- Password Generator

~ (v1.0.0.1)
Sabtu 6 April 2024 - First Release
#
<b>Panduan Cara Penggunaan:</b>
1. Pastikan sebelumnya sudah menginstal "Indihome Router Decoder Encoder" yang ada disini https://github.com/MichaelJorky/indihome-router-decoder
2. Download "Indihome Router Utility.exe" atau "iru-gui.exe" caranya arahkan cursor pada bagian "code" pada "local" pilih "download zip".
3. Pindahkan file yang sudah berhasil didownload pada folder ```.zte-decoder``` seperti yang sudah dibahas pada laman (point 1) lalu ekstract.
4. Untuk default script decodingnya maupun encodingnya menggunakan script seperti yang sudah dibahas pada (point 1) atau seperti yang tercantum dibawah ini:

<b>Default Decoder List (42 List):</b>
```
python autodecoder.py config/config.bin config/config.xml
python autodecoder.py --model "F670L" config/config.bin config/config.xml
python autodecoder.py --serial ZTEGCEFD0000 config/config.bin config/config.xml
python autodecoder.py --mac 60:E5:D8:00:00:00 --serial ZTEGCEFD0000 config/config.bin config/config.xml
python autodecoder.py --model "F670L" --serial ZTEGCEFD0000 config/config.bin config/config.xml
python decoder.py --key-prefix CEFD0000000000174654 --mac 60:E5:D8:00:00:00 --serial ZTEGCEFD0000 config/config.bin config/config.xml
python decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --mac 60:E5:D8:00:00:00 --serial ZTEGCEFD0000 config/config.bin config/config.xml
python decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --mac 60:E5:D8:00:00:00 --serial ZTEGCEFD0000 config/config.bin config/config.xml
python decoder.py --mac 60:E5:D8:00:00:00 --serial ZTEGCEFD0000 config/config.bin config/config.xml
python decoder.py --mac 60:E5:D8:00:00:00 --model "F670L" config/config.bin config/config.xml
python decoder.py --mac 60:E5:D8:00:00:00 --signature "ZXHN F670L V9.0" config/config.bin config/config.xml
python decoder.py --mac 60:E5:D8:00:00:00 --key '2bf3525fd2dcc7fe' config/config.bin config/config.xml
python decoder.py --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
python decoder.py --model "F670L" --serial ZTEGCEFD0000 config/config.bin config/config.xml
python decoder.py --model "F670L" --key '2bf3525fd2dcc7fe' config/config.bin config/config.xml
python decoder.py --model "F670L" --signature "ZXHN F670L V9.0" config/config.bin config/config.xml
python decoder.py --model "F670L" config/config.bin config/config.xml
python decoder.py --serial ZTEGCEFD0000 config/config.bin config/config.xml
python decoder.py --serial ZTEGCEFD0000 --key '2bf3525fd2dcc7fe' config/config.bin config/config.xml
python decoder.py --serial ZTEGCEFD0000 --signature "ZXHN F670L V9.0" config/config.bin config/config.xml
python decoder.py --key '2bf3525fd2dcc7fe' --signature "ZXHN F670L V9.0" config/config.bin config/config.xml
python decoder.py --key '2bf3525fd2dcc7fe' config/config.bin config/config.xml
python decoder.py --signature "F670L" config/config.bin config/config.xml
python decoder.py config/config.bin config/config.xml
python unidecoder.py --key-prefix CEFD0000000000174654 --try-all-known-keys --serial ZTEGCEFD0000 config/config.bin config/config.xml
python unidecoder.py --key-prefix CEFD0000000000174654 --signature "ZXHN F670L V9.0" --serial ZTEGCEFD0000 config/config.bin config/config.xml
python unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --try-all-known-keys --serial ZTEGCEFD0000 config/config.bin config/config.xml
python unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --signature "ZXHN F670 V9.0" --serial ZTEGCEFD0000 config/config.bin config/config.xml
python unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --try-all-known-keys --serial ZTEGCEFD0000 config/config.bin config/config.xml
python unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --signature "ZXHN F670 V9.0" --serial ZTEGCEFD0000 config/config.bin config/config.xml
python unidecoder.py --try-all-known-keys --signature "ZXHN F670L V9.0" --serial ZTEGCEFD0000 config/config.bin config/config.xml
python unidecoder.py config/config.bin config/config.xml
python unidecoder.py --longpass '' config/config.bin config/config.xml
python unidecoder.py --serial " " config/config.bin config/config.xml
python unidecoder.py --signature " " config/config.bin config/config.xml
python unidecoder.py --model " " config/config.bin config/config.xml
python unidecoder.py --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
python unidecoder.py --try-all-known-keys config/config.bin config/config.xml
python unidecoder.py --key '2bf3525fd2dcc7fe' config/config.bin config/config.xml
python unidecoder.py --serial ZTEGCEFD0000 config/config.bin config/config.xml
python unidecoder.py --model "F670L" config/config.bin config/config.xml
python unidecoder.py --signature "ZXHN F670L V9.0" config/config.bin config/config.xml
```
<b>Default Encoder List (23 List):</b>
```
python uniencoder.py --key-prefix CEFD0000000000174654 --signature "ZXHN F670L V9.0" --serial ZTE123456789 config/config.xml config/new.config.bin
python uniencoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --signature "ZXHN F670L V9.0" --serial ZTEGCEFD0000 config/config.xml config/new.config.bin
python uniencoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --signature "ZXHN F670L V9.0" --serial ZTEGCEFD0000 config/config.xml config/new.config.bin
python uniencoder.py --signature ZXHN F670L V9.0 --payload-type 0 config/config.xml config/new.config.bin
python uniencoder.py --signature ZXHN F670L V9.0 --payload-type 2 config/config.xml config/new.config.bin
python uniencoder.py --signature ZXHN F670L V9.0 --payload-type 4 config/config.xml config/new.config.bin
python uniencoder.py --signature ZXHN F670L V9.0 --payload-type 6 config/config.xml config/new.config.bin
python uniencoder.py --signature "ZXHN F670L V9.0" config/config.xml config/new.config.bin
python uniencoder.py --signature "ZXHN F670L V9.0" --version 1 --include-header config/config.xml config/new.config.bin
python uniencoder.py --signature "ZXHN F670L V9.0" --version 2 --include-header config/config.xml config/new.config.bin
python uniencoder.py --signature "ZXHN F670L V9.0" --include-unencrypted-length --include-header config/config.xml config/new.config.bin
python uniencoder.py --signature "ZXHN F670L V9.0" --use-signature-encryption config/config.xml config/new.config.bin
python uniencoder.py --signature "ZXHN F670L V9.0" --include-header config/config.xml config/new.config.bin
python uniencoder.py --serial ZTEGCEFD0000 --signature "ZXHN F670L V9.0" config/config.xml config/new.config.bin
python uniencoder.py --serial ZTEGCEFD0000 --signature " " config/config.xml config/new.config.bin
python uniencoder.py --serial ZTEGCEFD0000 --model "F670L" config/config.xml config/new.config.bin
python uniencoder.py --model "F670L" config/config.xml config/new.config.bin
python uniencoder.py --include-header --version 1 config/config.xml config/new.config.bin
python uniencoder.py --include-header --version 2 config/config.xml config/new.config.bin
python uniencoder.py --include-header --include-unencrypted-length config/config.xml config/new.config.bin
python uniencoder.py --include-header config/config.xml config/new.config.bin
python uniencoder.py --key '2bf3525fd2dcc7fe' --signature 'ZXHN F670L V9.0' --include-header config/config.xml config/new.config.bin
python uniencoder.py --key '2bf3525fd2dcc7fe' --signature 'ZXHN F670L V9.0' --version 1 --include-header config/config.xml config/new.config.bin
```
5. Untuk decoding support penggunaan perintah seperti contoh yang tercantum dibawah ini:
- --key 2bf3525fd2dcc7fe
- --model F670L
- --serial ZTEGCEFD0000
- --mac 60:E5:D8:00:00:00
- --longpass Telkomdso123
- --signature ZXHN F670L V9.0
- --key-prefix CEFD0000000000174654
- --iv-prefix ZTE%FN$GponNJ025
- --key-suffix 574ffbb30a488a9e2d583a86719400a7
- --iv-suffix dedb7b84041d5f10bfe84bca2a165e39
- --try-all-known-keys

6. Decoder yang dihasilkan dari "Decoder Generator" Total ada 0-11 Kombinasi:

~ 0 Kombinasi (3 List)
```
autodecoder.py config/config.bin config/config.xml
decoder.py config/config.bin config/config.xml
unidecoder.py config/config.bin config/config.xml
```
~ 1 Kombinasi (33 List)
```
autodecoder.py --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --model F670L config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --try-all-known-keys config/config.bin config/config.xml
decoder.py --model F670L config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --model F670L config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 config/config.bin config/config.xml
```
~ 2 Kombinasi (327 List)
```
autodecoder.py --signature ZXHN F670L V9.0 --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --model F670L --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --model F670L --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --model F670L config/config.bin config/config.xml
autodecoder.py --model F670L --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --model F670L config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --model F670L config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 --model F670L config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --model F670L config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --model F670L config/config.bin config/config.xml
autodecoder.py --model F670L --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 --model F670L config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --model F670L --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --model F670L config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --model F670L --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --try-all-known-keys --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 --try-all-known-keys config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --serial ZTEGCEFD0000 config/config.bin config/config.xml
autodecoder.py --model F670L --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --model F670L --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --key-prefix CEFD0000000000174654 --model F670L config/config.bin config/config.xml
autodecoder.py --mac 60:E5:D8:00:00:00 --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --longpass Telkomdso123 config/config.bin config/config.xml
autodecoder.py --model F670L --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --serial ZTEGCEFD0000 --model F670L config/config.bin config/config.xml
autodecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
autodecoder.py --signature ZXHN F670L V9.0 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --iv-prefix ZTE%FN$GponNJ025 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
autodecoder.py --model F670L --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --key 2bf3525fd2dcc7fe --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
autodecoder.py --longpass Telkomdso123 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --try-all-known-keys --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --try-all-known-keys --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --try-all-known-keys --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --model F670L --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 --try-all-known-keys config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --try-all-known-keys config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --try-all-known-keys config/config.bin config/config.xml
decoder.py --model F670L --try-all-known-keys config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --try-all-known-keys config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --try-all-known-keys --model F670L config/config.bin config/config.xml
decoder.py --model F670L --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --model F670L config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --try-all-known-keys config/config.bin config/config.xml
decoder.py --try-all-known-keys --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --try-all-known-keys --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --try-all-known-keys config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --model F670L config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --model F670L config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --try-all-known-keys config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --model F670L config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --try-all-known-keys config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --model F670L config/config.bin config/config.xml
decoder.py --model F670L --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --try-all-known-keys --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 --model F670L config/config.bin config/config.xml
decoder.py --try-all-known-keys --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --model F670L --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --try-all-known-keys --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --model F670L config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --model F670L --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --try-all-known-keys --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --try-all-known-keys config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --serial ZTEGCEFD0000 config/config.bin config/config.xml
decoder.py --model F670L --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --model F670L --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --key-prefix CEFD0000000000174654 --model F670L config/config.bin config/config.xml
decoder.py --mac 60:E5:D8:00:00:00 --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --longpass Telkomdso123 config/config.bin config/config.xml
decoder.py --model F670L --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --serial ZTEGCEFD0000 --model F670L config/config.bin config/config.xml
decoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
decoder.py --signature ZXHN F670L V9.0 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --iv-prefix ZTE%FN$GponNJ025 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
decoder.py --model F670L --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --key 2bf3525fd2dcc7fe --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
decoder.py --longpass Telkomdso123 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --model F670L --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --model F670L --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --model F670L config/config.bin config/config.xml
unidecoder.py --model F670L --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --model F670L config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --model F670L config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --model F670L config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --model F670L config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --model F670L config/config.bin config/config.xml
unidecoder.py --model F670L --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 --model F670L config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --model F670L --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --model F670L config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --model F670L --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --try-all-known-keys --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --try-all-known-keys config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --serial ZTEGCEFD0000 config/config.bin config/config.xml
unidecoder.py --model F670L --iv-prefix ZTE%FN$GponNJ025 config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --model F670L --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --key-prefix CEFD0000000000174654 --model F670L config/config.bin config/config.xml
unidecoder.py --mac 60:E5:D8:00:00:00 --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --key-suffix 574ffbb30a488a9e2d583a86719400a7 --longpass Telkomdso123 config/config.bin config/config.xml
unidecoder.py --model F670L --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --serial ZTEGCEFD0000 --model F670L config/config.bin config/config.xml
unidecoder.py --iv-suffix dedb7b84041d5f10bfe84bca2a165e39 --signature ZXHN F670L V9.0 config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
unidecoder.py --signature ZXHN F670L V9.0 --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --iv-prefix ZTE%FN$GponNJ025 --key 2bf3525fd2dcc7fe config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --key-prefix CEFD0000000000174654 config/config.bin config/config.xml
unidecoder.py --model F670L --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --key 2bf3525fd2dcc7fe --key-suffix 574ffbb30a488a9e2d583a86719400a7 config/config.bin config/config.xml
unidecoder.py --longpass Telkomdso123 --mac 60:E5:D8:00:00:00 config/config.bin config/config.xml
```
6. Encoder yang dihasilkan dari "Encoder Generator" (Segera):
```
Segera
```
