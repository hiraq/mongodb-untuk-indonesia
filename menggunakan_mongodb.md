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

Artinya, MongoDB memiliki skema yang fleksibel. Anda tidak dituntut untuk menentukan struktur data pada saat pembuatan collection. Layaknya folder, Anda dapat menempatkan apapun pada folder tersebut, seperti dokumen, gambar, lagu, atau apapun yang Anda inginkan.

Contoh membuat collection.

    db.createCollection('provinsi')


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

















