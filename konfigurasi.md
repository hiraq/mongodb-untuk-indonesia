# Konfigurasi

File konfigurasi berisi pengaturan yang secara fungsional sama dengan argumen yang ada pada `mongod` dan `mongos` di terminal. File konfigurasi digunakan agar lebih memudahkan dalam pengelolaan, terutama pada penyebaran skala besar. File konfigurasi memungkinkan komentar untuk menjelaskan alasan di balik pengaturan server tersebut.
    
Untuk `mongod`, dapat dijalankan dengan menggunakan :

    mongod --config /mongodb/mongodb.conf
    

Untuk `mongos`, dapat dijalankan dengan menggunakan :

    mongos -f /mongodb/mongodb.conf
    