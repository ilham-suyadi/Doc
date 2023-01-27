# Mengupload image ke docker hub

1. buat akun docker hub
2. buat repository di docker hub
3. buat image di docker dengan name *(username)/(name-repository):tag* jika sudah ada imagenya maka cukup ubah namanya dengan perintah *docker tag (name/id image) (name yang di inginkan):(tag), jika belum ada bisa mengcommit container jika dalam bentuk container
4. jika sudah selanjutnya adalah mengupload/mengepush image ke docker container
5. untuk push pastikan docker sudah login ke docker hub, jika belum bisa mengetikan *docker login* , nanti akan di suruh memasukkan username dan password
6. setelah login bisa mengepush image dengan perintah *docker push (username)/(name repository):(tag)*

> :link: Referensi <https://www.youtube.com/watch?v=HCXiB4pMuXU&list=PL-CtdCApEFH-A7jBmdertzbeACuQWvQao&index=16>
