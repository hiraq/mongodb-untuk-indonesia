# Menjalankan MongoDB

`mongod` adalah daemon utama untuk sistem MongoDB. Tugas `mongod` adalah menangani semua permintaan  dan pengelolaan data.

`mongod` membutuhkan direktori khusus untuk menyimpan data file. Secara default, direktori untuk `mongod` berada di `/data/db`, tetapi Anda dapat menentukan direktori sendiri untuk `mongod`.

Setelah menentukan direktori `mongod`, ubah permission direktori tersebut agar dapat membaca dan menulis. Pastikan juga bahwa MongoDB `bin` ada dalam variable PATH.


Menjalankan `mongod`.

    mongod

Jika menginginkan menjalankan MongoDB pada direktori yang berbeda, dapat menambahkan `--dbpath`. Jangan lupa untuk mengubah permission direktori tersebut agar dapat membaca dan menulis.

    mongod --dbpath /folder/yang/akan/dipakai