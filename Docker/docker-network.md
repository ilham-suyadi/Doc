# Docker Network

## Melihat Daftar Docker Network

```sh
docker network ls
```

## Membuat docker network Baru

```sh
docker network create (name network)
```

## menghapus docker network

```sh
docker network rm (name network)
```

## Melihat Detail dari network

```sh
docker inspect (name network)
```

## menambahkan network di container

```sh
docker container run -d --name (name container) --network (name network) (image) 
```
