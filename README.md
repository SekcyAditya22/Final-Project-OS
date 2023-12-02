NAMA  : Muhammad Aditya Madjid
NIM   : 22.83.0885

Menampilkan Pemeseanan Portofolio Web saya menggunakan WebServer dan Lainnya.
Saya memiliki Server Ubuntu dengan IP : 147.139.214.214

- ✨Portofolio WEB ✨
- HTML
- CRUD

## Service

- Web Server (Apache2, MySQL, PHP)
- SSH
- FTP
- Montitoring Server
- 

## Instalasi Web Server

1. Update dan upgrade ubuntu terlebih dahulu
   ```bash
   sudo apt update
   sudo apt upgrade 
   ```

2. Install Apache2 untuk Web Servernya
   ```bash
   sudo apt install apache2
   ```
   Test pada Browser apakah sudah terkoneksi.

3. Install Tambahan untuk libapache2 PHP Mysql
   ```bash
   sudo apt install php libapache2-mod-php php-mysql
   ```

4. Mengizinkan Firewall untuk Apache2 pada port 80 dan port 80/tcp
   ```bash
   ufw allow 80
   ufw allow 80/tcp
   systemctl restart apache2
   ```

5. Start, Enable, Restart Apache2
   ```bash
   systemctl start apache2
   systemctl enable apache2
   systemctl restart apache2
   ```

6. Install phpMyAdmin
   ```bash
   sudo apt install phpmyadmin
   ```

7. Mengaktifkan Ekstensi PHP yang digunakan
   ```bash
   sudo phpenmod mbstring
   ```

8. Restart apache2
   ```bash
   systemctl restart apache2
   ```

9. Install mysql untuk database
   ```bash
   sudo apt install mysql-server
   ```

10. Konfigurasi Akun mysql untuk menuju ke phpMyAdmin
    ```bash
    sudo mysql -u root -p
    ```

    Membuat User/Akun untuk mysql database
    ```sql
    ALTER USER 'root'@'localhost' IDENTIFIED WITH 'mysql_native_password' BY 'isikan_password' ;
    ```
    ```sql
    FLUSH PRIVILEGES;
    ```
    ```sql
    exit;
    ```

    Restart MySQL dan phpMyAdmin
    ```bash
    systemctl restart mysql
    systemctl restart phpmyadmin
    ```

## Instalasi SSH

1. Install Service SSH pada Ubuntu
   ```bash
   sudo apt install openssh-server
   ```

2. Mengizinkan Firewall untuk SSH dengan port 22 dan 22/tcp
   ```bash
   ufw allow 22
   ufw allow 22/tcp
   ```

3. Konfigurasi SSH sesuai keinginan pada:
   ```bash
   nano /etc/ssh/sshd_config
   ```
   Dapat disetting PermitLogin root atau Pengubahan Port yang diinginkan

4. Start, Enable, Restart SSH
   ```bash
   systemctl start ssh
   systemctl enable ssh
   systemctl restart ssh
   ```



    


    
