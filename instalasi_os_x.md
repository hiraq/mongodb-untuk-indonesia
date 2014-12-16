# Instalasi - OS X

Ada dua cara instalasi pada OS X, yaitu :

- Via [Homerew](http://brew.sh/)
- Manual

## Homebrew

Instalasi MongoDB production release

    brew install mongodb
    
Instalasi dengan dukungan SSL, dapat menambahkan `--with-openssl`

    brew install mongodb --with-openssl

Instalasi MongoDB development release, dapat menambahkan `--devel`

    brew install mongodb --devel
    
    
## Manual

Unduh file dari `https://www.mongodb.org/downloads`.

    curl -O http://downloads.mongodb.org/osx/mongodb-osx-x86_64-2.6.6.tgz

Ekstrak file

    tar -zxvf mongodb-osx-x86_64-2.6.6.tgz

Ubah nama folder `mongodb-osx-x86_64-2.6.6` menjadi `mongodb`.

    mv mongodb-osx-x86_64-2.6.6 mongodb

Tambahkan MongoDB pada variabel PATH

    export PATH=<FOLDER MONGODB>/bin:$PATH


















