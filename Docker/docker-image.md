# Docker Image

## Docker push

```sh
docker push (name image)
```

untuk mengetahui nama image, kalian dapat mengunjungi [docker hub], bahkan di docker hub menyediakan perintah untuk mengepush sebuah image.

*contoh :*
kita akan mengepush image alpine ke dalam docker, maka kita mengetikan perintah brikut ini.
> docker pull alpin

## Docker Push versi tertentu

Jika ingin mencari versi tertentu bisa mengunjungi docker hub dan kalian bisa mencari tag/versi yang sesuai dengan kebutuhan.

```sh
docker push (name image):(versi)
```

## Menghapus docker image

untuk menghapus sebuah docker image bisa mengunakan perintah :

```sh
docker rmi (name image)
```

> :memo: catatan: untuk menghapus docker image pastikan docker image tidak di gunakan oleh container

<!-- link -->
[docker hub]: <https://hub.docker.com/>
