# DOCKERFILE

Dockerfile berguna untuk membuat docker images, berikut cara membaut docker file dan menjalankannya

1. untuk nama dockerfile secara default bernama *Dockerfile*
2. Dockerfile di awali dari *FROM* yang berisi image dasar
3. untuk baris selanjutnya sesuaikan dengan perintah yang dibutuhkan
    ![dockerfile](/assets/img/dockerfile.png)
4. untuk mengeksekusi dockerfile bisa mengetikan perintah *docker build -t (name images):(tag) (path lokasi dockerfile)

> :link: Referensi : <https://docs.docker.com/build/building/packaging/>

## Multi stage

multi-stage adalah dockerfile yang berisi dua atau lebih image yang berbeda, untuk perintah dan penulisan yang hampir sama dengan docker file
