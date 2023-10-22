* SYSADMIN
  1. Menginstall Web Server LAMP menggunakan web server apache2
  2. Kemudian diikuti dengan service berupa ssh dan ftp serta virtual dns dan web yang saya buat
  3. Saya menggunakan web server untuk web html.
  4. Yang diatas sudah saya lakukan semua.
  5. Sudah berjalan secara lokal area saja

* OS SERVER
  Untuk Operasi Sistem yang digunakan menggunakan Linux Ubuntu 20.04, karena yang lebih ringan dan sudah lumayan lengkap untuk digunakan. 
-	Web Server sendiri menggunakan Apache2 dikarenakan:
Memakai apache2 karena modularitas yang lebih banyak pilihannya 
Keamanan pada izin akses yang memadai
Dukungan pembacaan bahasa pemrograman yang banyak

-	Mysql dan phpMyAdmin 
Digunakan untuk manajemen basis data dan pengembangan aplikasi web.
(Menginstall Mysql dan PhpMyAdmin

-	Bahasa PHP
Untuk membaca basis data dan database yang akan dilakukan.


Lalu dilanjutkan dengan beberapa service yang diperlukan.
-	SSH 
Untuk melakukan remote server kita dengan metode jarak jauh agar dapat diakses dimana saja Ketika dibutuhkan. (Menggunakan Service SSH sshd pada Linux Ubuntu

-	FTP
Mentransfer data html dan lainnya agar memudahkan saya untuk melakukan pertukaran data yang banyak. (Menggunakan vsftpd pada Linux Ubuntu)

-	DNS
Pemberian Domain Name Server yang berfungsi untuk memberikan nama domain pada ip browser html saya. (Menggunakan Bind9)



-	Monitoring Server
Untuk memantau aktivitas server baik log server maupun memantau hardware pada server. (Menggunakan Prometheus, promtail, dan Grafana).

-	Service HTML optional
Menggunakan SSL untuk mengamankan dan mengenkripsi web.

  
