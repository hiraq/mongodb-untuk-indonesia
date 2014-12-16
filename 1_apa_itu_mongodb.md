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


## Pemetaan

### Terminologi dan Konsep

Tabel berikut menyajikan terminologi berbagai SQL dan MongoDB.

<table>
    <colgroup>
        <col width="50%">
            <col width="50%">
    </colgroup>
    <thead>
        <tr>
            <th>SQL</th>
            <th>MongoDB</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>database</td>
            <td>database</td>
        </tr>
        <tr>
            <td>table</td>
            <td>collection</td>
        </tr>
        <tr>
            <td>row</td>
            <td>document</td>
        </tr>
        <tr>
            <td>column</td>
            <td>field</td>
        </tr>
        <tr>
            <td>index</td>
            <td>index</td>
        </tr>
        <tr>
            <td>table joins</td>
            <td>embedded documents dan linking</td>
        </tr>
        <tr>
            <td>primary key</td>
            <td>primary key</td>
        </tr>
    </tbody>
</table>


### Executables

Database server menggunakan `mongod` dan client	menggunakan `mongo`.












