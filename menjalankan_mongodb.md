# Menjalankan MongoDB

`mongod` adalah daemon utama untuk sistem MongoDB. Tugas `mongod` adalah menangani semua permintaan  dan pengelolaan data.

`mongod` membutuhkan direktori khusus untuk menyimpan data file. Secara default, direktori untuk `mongod` berada di `/data/db`, tetapi Anda dapat menentukan direktori sendiri untuk `mongod`.

Setelah menentukan direktori `mongod`, ubah permission direktori tersebut agar dapat membaca dan menulis.

Menjalankan `mongod`.

    mongod

Jika menginginkan menjalankan MongoDB pada direktori yang berbeda, dapat menambahkan `--dbpath`.

    mongod --dbpath /folder/yang/akan/dipakai
    
