# MongoDB

MongoDB merupakan open-source document database dari keluarga [NoSQL](http://id.wikipedia.org/wiki/NoSQL), yang memberikan kinerja tinggi, high availability, dan automatic scaling.

## Document
Data pada MongoDB dikenal sebagai document. MongoDB menggunakan [BSON](http://bsonspec.org/) sebagai format penyimpanan data untuk document, mirip dengan JSON.

Contoh document

    {
       "_id": ObjectId("549081be0dbcfd82140041a7"),
       "nama": "Wahyu Kristianto",
       "nomor": NumberLong(12345),
       "bahasa": [
         "bahasa",
         "english" 
      ] 
    }


## Terminologi dan Konsep