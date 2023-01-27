# Add Gmail di Gitlab

sebelum kita menambahkan akun gmail ke dalam gitlab, kita harus menyetting beberapa hal yang ada di gmail kita.

## Mengatur Gmail

1. kita masuk ke [my account google], pastikan kita sudah masuk masuk ke akun gmail kita.
2. klik keaman atau security, dan scroll ke bawah sampai ke login gmail.
   ![01]
3. yang kita atur :

    >1. mengatur verifikasi 2 langkah.
    >
    >- klik verifikasi 2 langkah
    >- setelah itu kita disuruh memasukkan kata sandi gmail kita
    >- maka kita akan di di beri beberapa opsi untuk masuk ke akun gmail
    >- untuk lengkapnya kalian dapat menonton <https://www.youtube.com/watch?v=n0EenvoBNNg>
    >
    >2. sandi aplikasi.
    >
    >- klik sandi aplikasi
    >- setelah itu kita akan di bawa masuk ke sandi aplikasi
    >- di sandi aplikasi, kita pilih yang bawah, dan klik pilih aplikasi dan *pilih lainnya (nama kustom)*
    >- setelah itu kita masukkan nama, untuk nama itu bebas, tapi disini saya menggunakan *gitlab-gmail*, jika sudah maka tekan buat.
    >- setelah itu akan muncul kata sandi yang nanti kita gunakan untuk gitlab, saya sarankan anda mengcopy sandi perangkat anda.
    >- setelah itu nama yang telah kita buat akan muncul di sandi aplikasi.
    [video tutorial]

4. mengkonfigurasi gitlab di docker :
    >
    > - masuk ke gitlab bash dengan perintah *docker exec -it gitlab*
    > - mengubah/mengedit gitlab.rb, untuk masuk ke gitlab.rb dapat mengetikkan perintah *vi /etc/gitlab/gitlab.rb*
    > - sesuaikan script dengan gambar di bawah ini
    > - ![02](/assets/img/Screenshot_14.png)
    > - dan reconfigure gitlab dengan perintah *gitlab-ctl reconfigure*
<!-- link -->
[my account google]: <https://myaccount.google.com/>
[video tutorial]: <https://www.youtube.com/watch?v=pAPWBHxnFHM>
[01]: </assets/img/01.png>

<!-- </img src="/assets/img/03.png" style=" width:560px ; height: 400px"> -->