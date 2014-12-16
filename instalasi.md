# Instalasi, Menjalankan dan Konfigurasi MongoDB

## Instalasi

Untuk proses instalasi, pilih sistem operasi yang digunakan.

* [OS X](instalasi_os_x.md)


## Menjalankan MongoDB

Sebelum menjalankan MongoDB, buatlah direktori khusus untuk `mongod` yang akan melakukan proses menulis data. Defult direktori berada di `/data/db`. Ubah permission direktori tersebut agar dapat membaca dan menulis, dan pastikan bahwa MongoDB `bin` ada dalam variable PATH.


Jalankan `mongod`.

    mongod

Jika menginginkan menjalankan MongoDB pada direktori yang berbeda, dapat menambahkan `--dbpath`. Jangan lupa untuk mengubah permission direktori tersebut agar dapat membaca dan menulis.

    mongod --dbpath /folder/yang/akan/dipakai
    
    

## Konfigurasi MongoDB
    
File konfigurasi berisi pengaturan yang secara fungsional sama dengan argumen `mongod` dan `mongos` pada terminal. File konfigurasi digunakan agar lebih mudah pengelolaan, terutama pada penyebaran skala besar. File konfigurasi memungkinkan komentar untuk menjelaskan alasan di balik pengaturan server tersebut.
    
Untuk `mongod`

    mongod --config /mongodb/mongodb.conf
    

Untuk `mongos`

    mongos -f /mongodb/mongodb.conf
    
    
    
    
    
    
    