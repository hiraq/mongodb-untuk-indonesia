# Instalasi dan Menjalankan MongoDB

## Instalasi

Untuk proses instalasi, pilih sistem operasi yang digunakan.

* [OS X](instalasi_os_x.md)


## Menjalankan MongoDB

Sebelum menjalankan MongoDB, buatlah direktori khusus untuk `mongod` yang akan melakukan proses menulis data. Ubah permission direktori tersebut agar dapat membaca dan menulis.

*Asumsi direktori berada di `/data_mongodb`*.

Jalankan `mongod`. Pastikan bahwa MongoDB `bin` ada dalam variable PATH.

    mongod

