# Instalasi dan Menjalankan MongoDB

## Instalasi

Untuk proses instalasi, pilih sistem operasi yang digunakan.

* [OS X](instalasi_os_x.md)


## Menjalankan MongoDB

Sebelum menjalankan MongoDB, buatlah direktori khusus untuk `mongod` yang akan melakukan proses menulis data. Defult direktori berada di `/data/db`. Ubah permission direktori tersebut agar dapat membaca dan menulis, dan pastikan bahwa MongoDB `bin` ada dalam variable PATH.


Jalankan `mongod`.

    mongod

Jika menginginkan menjalankan MongoDB pada direktori yang berbeda, dapat menambahkan `--dbpath`. Jangan lupa untuk mengubah permission direktori tersebut agar dapat membaca dan menulis.

    mongod --dbpath /folder/yang/akan/dipakai