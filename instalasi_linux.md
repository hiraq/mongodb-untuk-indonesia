# Instalasi - Linux

Di step ini, menggunakan linux distro dari turunan Debian, yaitu Ubuntu.  Ada dua cara dalam proses instalasi, yaitu :

- Via package manager (apt-get)
- Manual

## Via Package Manager (apt-get)

  ```
  sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10
  ```
  
  ```
  echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' | sudo tee /etc/apt/sources.list.d/mongodb.list
  ```
  
  ```
  sudo apt-get update
  ```
  
  ```
  sudo apt-get install mongodb-org
  ```
  
## Via Manual

  ```
  //download
  wget https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-2.6.6.tgz?_ga=1.141304754.144130295.1420197961
  ```
  
  ```
  //extract 
  tar -zxvf mongodb-linux-x86_64-2.6.6.tgz
  ```
  
  ```
  mv mongodb-linux-x86_64-2.6.6 mongodb
  ```
  
  ```
  export PATH=<FORDER_MONGODB>/bin:$PATH
  ```
  
Lebih baik menggunakan package manager, karena dengan cara ini, kita sudah termasuk mendapatkan control script, yaitu sebuah script untuk mengatur mongodb agar bisa berjalan sebagai sebuah daemon, termasuk pengontrolan untuk start & stop
