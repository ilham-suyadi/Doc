# membuat directory yang bisa diakses oleh grup yang sama

1. masuk ke mode root
2. yang pertama adalah membuat grup, untuk membuat grup masukkan perintah *groupadd (name group)*
3. setelah membuat grup, maka langkah selanjutnya adalah memasukkan user kedalam group dengan perintah *usermod -aG (name group) (name user)*
4. langkah berikutnya membuat directory, untuk directory saya letakan di relative patch yang ditandai dengan slash (/), directory di relative patch sebenarnya hanya bisa diakses oleh root, kecuali home. nah dalam kasus ini kita akan membuat sebuah directory di relative patch, yang bisa di akses oleh group tertentu.
5. untuk membuatnya directory langkah awal adalah pindah ke directory patch dengan perintah *cd /*
6. setelah itu membuat directory, dengan perintah *mkdir (name folder)*
7. memberi akses pada folder dengan perintah *chmod 770 (name file)*
8. memasukkan directory ke group, dengan perintah *chgrp (name group) (name file)*
9. jika sudah maka file tersebut dapat diakses oleh grup yang di ijinkan

> :memo: Catatan: pastikan file yang di upload di group tersebut sudah diatur ijinnya dengan cara *chmod 770 (name file)*, kalau tidak maka file tersebut akan terkunci atau tidak bisa di edit oleh orang lain
