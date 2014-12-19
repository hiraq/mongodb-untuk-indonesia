# Instalasi - OS X

Ada dua cara instalasi pada OS X, yaitu :

- Via [Homerew](http://brew.sh/)
- Manual

## Via Homebrew

Instalasi MongoDB production release

    brew install mongodb
    
Instalasi dengan dukungan SSL, dapat menambahkan `--with-openssl`

    brew install mongodb --with-openssl

Instalasi MongoDB development release, dapat menambahkan `--devel`

    brew install mongodb --devel
    
    
## Manual

Unduh file dari `https://www.mongodb.org/downloads`. Contoh yang digunakan saat ini adalah MongoDB versi 2.6.6 / 64-bit.

    curl -O http://downloads.mongodb.org/osx/mongodb-osx-x86_64-2.6.6.tgz

Ekstrak file

    tar -zxvf mongodb-osx-x86_64-2.6.6.tgz

Ubah nama folder `mongodb-osx-x86_64-2.6.6` menjadi `mongodb`.

    mv mongodb-osx-x86_64-2.6.6 mongodb

Tambahkan MongoDB pada [PATH environment variable](http://en.wikipedia.org/wiki/PATH_%28variable%29)

    export PATH=<FOLDER MONGODB>/bin:$PATH


















