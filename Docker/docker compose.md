# docker compose

docker compose berguna untuk membuat sebuah container

## 1. nama file untuk docker compose

docker compose secara default bernama docker-compose.yml, tapi docker compose juga bisa menjalankan file dengan nama lain asalkan menggunakan ekstensi *.yml*. ***cth :*** install-gitlab.yml, nginx.yml

## 2. penulisan perintah di docker compose (.yml)

> 1. diawali dengan version, biasanya saya menggunakan *3.8* atau *3*.
> ***dengan Format Penulisan :*** version: '3.8'
>
> 2. setelah menuliskan version, selanjutnya adalah menuliskan perintah services, service wajib ditulis karena awal dari mulainya perintah di docker compose.
> ***format penulisan :*** services :
>
> 3. selanjutnya membuat nama untuk proses tersebut di bawah service, pastikan nama untuk proses itu berjarak dengan services :
> ***cth :*** web: db:
> 4. di dalam nama operasi terdapat image yang akan digunakan, pastikan kita harus memberi jarak 1 tab lebih ke dalam  daripada name operasi.
> ***dengan format penulisan :***   image: (name image)
> ![01](/assets/img/docker-compose-01.png)
>5. setelah itu semuanya bersifat opsional.
>6. contoh penulisan :
>
>
>![03](/assets/img/docker-compose-03.png)
>
> > :memo: Catatan : docker compose memperhatikan map/tap/struktur yang digunakan dalam penulisan

## 3. menjalankan perintah yang ada di docker compose yml

 jika file tersebut bernama `docker-compose.yml` maka dapat menjalankan perintah :

 ```sh
 docker compose up -d
 ```

atau jika file tersebut bernama lain tapi berekstensi `.yml` maka menjalankan perintah :

```sh
docker compose -f (name-file).yml up -d
