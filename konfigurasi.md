# Konfigurasi


File konfigurasi MongoDB menggunakan format [YAML](http://www.yaml.org/), berisi pengaturan yang secara fungsional sama dengan argumen yang ada pada `mongod` dan `mongos` yang dijalankan pada terminal. File konfigurasi digunakan agar lebih memudahkan dalam pengelolaan, terutama pada penyebaran skala besar, dan memungkinkan komentar untuk menjelaskan alasan di balik pengaturan server tersebut.
    
Untuk menjalankan `mongod` dengan menggunakan konfigurasi yang berada di `/mongodb/mongodb.conf`, dapat dilakukan seperti yang ada di bawah ini.

    mongod --config /mongodb/mongodb.conf


Hal yang sama, dapat dijalankan untuk `mongos`. Contoh di bawah ini menggunakan `-f` alias dari `--config`.

    mongos -f /mongodb/mongodb.conf
    

*Lihat lebih lanjut kumpulan opsi yang dapat digunakan untuk [`mongod`](http://docs.mongodb.org/manual/reference/program/mongod/) dan [`mongos`](http://docs.mongodb.org/manual/reference/program/mongos/)*.
