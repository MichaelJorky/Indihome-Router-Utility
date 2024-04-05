# Indihome Router Utility (iru-gui.exe)

Indihome Router Utility adalah alat Decoder dan Encoder config pada router seperti zte, huawei, tp-link, d-link, tenda, fiberhome dll dan alat ini baru disempurnakan untuk router zte, dengan alat ini Anda tidak perlu bersusah payah untuk mencari seputar isi konfigurasi pada router di rumah Anda.
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
1. Pastikan sebelumnya sudah menginstal "indihome router decoder" yang ada disini https://github.com/MichaelJorky/indihome-router-decoder
2. Download "Indihome Router Utility.exe" atau "iru-gui.exe" caranya arahkan cursor pada bagian "code" pada "local" pilih "download zip".
3. Pindahkan file yang sudah berhasil didownload pada folder ```.zte-decoder``` seperti yang sudah dibahas pada laman (point 1) lalu ekstract.
4. Untuk default script decodingnya maupun encodingnya menggunakan script seperti yang sudah dibahas pada (point 1) atau seperti yang tercantum dibawah ini:

<b>Default Decoder List:</b>
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
python decoder.py --key 'Telkomdso123' --signature "ZXHN F670L V9.0" config/config.bin config/config.xml
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
python unidecoder.py --serial ZTE123456789 config/config.bin config/config.xml
python unidecoder.py --model "F670L" config/config.bin config/config.xml
python unidecoder.py --signature "ZXHN F670L V9.0" config/config.bin config/config.xml
```
<b>Default Encoder List:</b>
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


