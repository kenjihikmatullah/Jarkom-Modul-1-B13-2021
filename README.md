# Jarkom-Modul-1-B13-2021

**Members**
- Abdulatif Fajar Sidiq
- Kenji Hikmatullah (05111840000074)


#### 1. Sebutkan webserver yang digunakan pada "ichimarumaru.tech"! 

Filter ekspression : *http.post==ichimarumaru.tech*

Server: *nginx/1.18.0 (Ubuntu)*

![Screenshot](/screenshots/1-0.png)

#### 2. Temukan paket dari web-web yang menggunakan basic authentication method!

*http.authbasic*

![Screenshot](/screenshots/2-0.png)

#### 3. Ikuti perintah di basic.ichimarumaru.tech! Username dan password bisa didapatkan dari file .pcapng!

*Username dan password kuncimenujulautan:tQKEJFbgNGC1NCZlWAOjhyCOm6o3xEbPkJhTciZN*

![Screenshot](/screenshots/3-0.png)

#### 4. Temukan paket mysql yang mengandung perintah query select!

*mysql.query contains "select"*

![Screenshot](/screenshots/4-0.png)

#### 5. Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan password bisa didapat dari query insert pada table users dari file .pcap!

*mysql.query contains "INSERT"*

![Screenshot](/screenshots/5-0.png)

![Screenshot](/screenshots/5-1.png)

#### 6. Cari username dan password ketika melakukan login ke FTP Server!

*ftp.request.command =="USER" || ftp.request.command == "PASS"*

![Screenshot](/screenshots/6-0.png)

![Screenshot](/screenshots/6-1.png)

#### 7. Ada 500 file zip yang disimpan ke FTP Server dengan nama 0.zip, 1.zip, 2.zip, ..., 499.zip. Simpan dan Buka file pdf tersebut. (Hint = nama pdf-nya "Real.pdf")

*frame contains "Real.pdf"*

![Screenshot](/screenshots/7-0.png)

![Screenshot](/screenshots/7-1.png)

![Screenshot](/screenshots/7-2.png)


#### 8. Cari paket yang menunjukan pengambilan file dari FTP tersebut!

*ftp.request.command contains "GET" || ftp.request.command contains "RETR"*

![Screenshot](/screenshots/8-0.png)

#### 9. Dari paket-paket yang menuju FTP terdapat inidkasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama "secret.zip". Simpan dan buka file tersebut!

*ftp.command contains "secret.zip"*

![Screenshot](/screenshots/9-0.png)

#### 10. Selain itu terdapat "history.txt" yang kemungkinan berisi history bash server tersebut! Gunakan isi dari "history.txt" untuk menemukan password untuk membuka file rahasia yang ada di "secret.zip"!

*ftp-data*

![Screenshot](/screenshots/10-0.png)

#### 11. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80! 

*port 80*

![Screenshot](/screenshots/11-0.png)

#### 12. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
*port 21*

![Screenshot](/screenshots/12-0.png)

#### 13. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!

*dst port 443*

![Screenshot](/screenshots/13-0.png)

#### 14. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!

*dst host 103.7.13.247*

![Screenshot](/screenshots/14-0.png)

#### 15. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

*src host 192.168.138.55*

![Screenshot](/screenshots/15-0.png)
