# Konfigurasi

File konfigurasi berisi pengaturan yang secara fungsional sama dengan argumen `mongod` dan `mongos` pada terminal. File konfigurasi digunakan agar lebih mudah pengelolaan, terutama pada penyebaran skala besar. File konfigurasi memungkinkan komentar untuk menjelaskan alasan di balik pengaturan server tersebut.
    
Untuk `mongod`

    mongod --config /mongodb/mongodb.conf
    

Untuk `mongos`

    mongos -f /mongodb/mongodb.conf
    