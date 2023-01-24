# Menginstal Git di CentOS

1. Perintah untuk menginstall git di centos :

   ```sh
   yum install git
   ```

  ![git install](/assets/img/Screenshot_2.png)

2. mengecek versi dari git yang kita install :

    ```sh
    git --version
    atau
    git -v
    ```

    ![git version](/assets/img/Screenshot_1.png)

## Mengupdate versi git menjadi versi 2

1. jika kita sudah pernah menginstal git, maka kita harus menghapus git dulu, untuk menghapus git dapat menjalan perintah:

   ```sh
   sudo yum -y remove git
   sudo yum -y remove git-*
   ```

   ![git remove](/assets/img/Screenshot_3.png)
   ![git remove](/assets/img/Screenshot_4.png)

2. jika sudah, maka selanjutnya adalah menambahkan repository dengan perintah :

     ```sh
    yum -y install https://packages.endpointdev.com/rhel/7/os/x86_64/endpoint-repo.x86_64.rpm
   ```

    ![git repo](/assets/img/Screenshot_7.png)

3. selanjutnya adalah menginstall git, perintah untuk untuk mengintall git :

    ```sh
   yum install git
   atau
   yum install git -y
   ```

   ![git installl](/assets/img/Screenshot_6.png)

4. cek versi :

    ```sh
    git --version
    atau
    git -v
    ```

    ![git versio 2](/assets/img/Screenshot_5.png)

> :memo: Catatan= yang membedakan proses instal git versi 1.8 dengan git versi 2, yaitu di bagian repository di git 1.8 kita tidak menmbahkan repository, sedangkan di versi 2 kita menambahkan repository baru seblum waktu penginstalan.

- :book: Refrensi untuk install git <https://www.vultr.com/docs/how-to-install-git-on-centos-7/>
- :book: Refrensi untuk install git versi 2 <https://computingforgeeks.com/install-git-2-on-centos-7/>
