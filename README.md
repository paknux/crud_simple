# Aplikasi CRUD Simple 

## Langkah Kerja

### A. Buat Security Group

1. Buat security group server web : 

    sg-webserver
    
    ```allow inbound 22,80, ICMP from 0.0.0.0/0 (anywhere)```


2. Buat security group database SQL : 

    sg-database
    
    ```allow inbound 3306 from 0.0.0.0/0 (anywhere)```

### B. Buat RDS
### C. Buat Mesin (Instance EC2) Ubuntu

