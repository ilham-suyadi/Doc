# Docker Container

## Docker Run

docker run berguna untuk untuk membuat dan menjalankan sebuah container yang berasal dari docker image

```sh
docker run (name image)
```

## Menjalankan Docker Run di latar belakang

jika kita menjalankan perintah docker run maka proses pembuatannya berjalan di layar depan, dan itu akan berjalan terus-menerus jika tidak di stop, jika ingin menjalankan proses docker run di latar belakang kita bisa menambahkan ***-d***, berikut contohnya:

```sh
docker run -d (name image)
```

## Mengatur Nama untuk Docker Container

```sh
docker run -d --name (name container) (name image)
```

## Mempublish Port Docker container

```sh
docker run -d --name (name container) -p (port yang kita inginkan):(port dari aplikasi) (name image)
```

## Docker start

```sh
docker start (name container/id container)
```

## Docker Stop

```sh
docker stop (name container/id container)
```

## Docker rm

```sh
docker rm (name container/id container)
```

## Menghapus semua container yang bersestatus exit

```sh
docker rm $(docker ps -a -q -f status=exited)
```

- status=exited : perintah ini akan menghapus semua docker container yang bersetatus exit/exited
- -q : hanya mengembalikan ID numerik
- -f : memfilter keluaran berdasarkan kondisi yang disediakan

## membersihkan docker

```sh
docker container prune
```
