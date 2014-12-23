# Menggunakan MongoDB

![status](https://dl.dropboxusercontent.com/u/83581209/mongodb-untuk-indonesia/button.status.dalam-pengembangan.png)


## Menjalankan `mongo`
Anda dapat menggunakan MongoDB dengan menjalankan `mongo`.

    mongo
    

Secara otomatis, `mongo` akan menggunakan database **test**.

![Menjalankan MongoDB](https://dl.dropboxusercontent.com/u/83581209/mongodb-untuk-indonesia/assets/menggunakan_mongodb.1.png)

## Database

Dengan MongoDB, Anda tidak perlu repot dengan membuat database terlebih dahulu. Anda dapat langsung menggunakan database yang Anda inginkan, sekalipun database tersebut belum dibuat.

Contoh berikut adalah menggunakan database **indonesia**.

    > use indonesia


*Penggunaan database lengkap, dapat dilihat di bab [Database](database.md)*

## Collection

Pengelompokan dokumen di MongoDB disebut collection. Jika Anda pernah menggunakan SQL sebelumnya, collection sama halnya dengan table. Anda dapat melihat Terminologi dan Konsep pada [halaman MongoDB](mongodb.md).

> MongoDB adalah schemaless!

Artinya, MongoDB memiliki skema yang fleksibel. Layaknya folder, Anda dapat menempatkan apapun pada folder tersebut, seperti dokumen, gambar, lagu, atau apapun yang Anda inginkan. Anda tidak dituntut untuk menentukan struktur data pada saat pembuatan collection, dan dapat menempatkan data dengan struktur yang berbeda-beda.

Contoh membuat collection.

    db.createCollection('provinsi')

*Penggunaan collection lengkap, dapat dilihat di bab [Database](database.md) dan [Collection](collection.md)*

## Document

Document akan sering Anda jumpai. Disinilah data yang akan Anda kelola.


### Manambahkan Document

Dibawah ini adalah contoh untuk menambahkan document baru pada collection "**provinsi**".

    db.provinsi.insert({ nama: "DKI Jakarta" })
    
Anda dapat menambahkan document lainnya dengan struktur yang berbeda.

    db.provinsi.insert({ nama: "Aceh", ibukota: "Banda Aceh" })
    

### Mencari Document

Setelah Anda menambahkan document pada collection, kali ini Anda akan dipandu untuk mencari document yang telah Anda buat sebelumnya.

Mencari seluruh document.

    db.provinsi.find()

Anda akan memperoleh hasil seperti ini.

![Mencari Document](https://dl.dropboxusercontent.com/u/83581209/mongodb-untuk-indonesia/assets/menggunakan_mongodb.2.png)


### Mengubah Document

Data yang sudah dibuat, dapat diubah kembali. Ada dua jenis pengubahan data, yaitu :

- Mengubah spesifik field pada document,
- Mengganti document.


#### Mengubah spesifik field pada document

`$set` dapat digunakan untuk mengubah hanya pada spesifik field.

Contoh berikut adalah untuk mengubah field "nama" dari "DKI Jakarta" ke "Jakarta".

    db.provinsi.update(
        { nama: "DKI Jakarta" },
        {
          $set: {
            nama: "Jakarta"
          }
        }
    )
    
    
#### Mengganti document

Anda juga dapat mengganti document yang sudah ada dengan document baru. Perbedaannya adalah, seluruh field yang ada pada document yang sudah ada, akan diganti dengan seluruh field yang baru.


    db.provinsi.update(
       { nama: "Jakarta" },
       { ibukota: "Jawa Barat" }
    )

![Mengubah Document](https://dl.dropboxusercontent.com/u/83581209/mongodb-untuk-indonesia/assets/menggunakan_mongodb.3.png)


### Menghapus Document



*Penggunaan collection lengkap, dapat dilihat di bab [Collection](collection.md) dan [Cursor](cursor.md)*












