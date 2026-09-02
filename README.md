# Aplikasi CRUD Simple 

## Langkah Kerja

### A. Buat Security Group
 
1. Buat security group server web : 

    webserver-sg
    
    ```allow inbound SSH (22), HTTP (80), dan ICMP from 0.0.0.0/0 (anywhere)```


2. Buat security group database SQL : 

    database-sg
    
    ```allow inbound MySQL (3306) from 0.0.0.0/0 (anywhere)```

### B. Buat RDS
### C. Buat Mesin (Instance EC2) Ubuntu

1. Masuk dapat menggunakan SSM
    ```bash
    $  bash 
    $  sudo su
    #
    ```


2. Install Paket yang diperlukan
    ```bash
    #  apt update
    #  apt install git apache2 php php-mysqli php-mysql libapache2-mod-php
    ```

3. Masuk ke DocumentRoot dan hapus semua isinya
    ```bash
    #  cd /var/www/html
    #  rm -rf *
    #  rm -rf .*
    ```