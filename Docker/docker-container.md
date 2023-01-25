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

## Docker Stop

## Docker rm
