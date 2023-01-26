# volume

volume adalah storage container, yang di simpan di docker.

## melihat volume

```sh
docker volume ls
```

## membuat docker volume

```sh
docker volume create (name volume)
```

## menghapus docker volume

```sh
docker volume rm (name volume)
```

> :memo: pastikan volume tidak di gunakan container

## menghubungkan container dengan volume

```sh
docker container run -d --mount 'type=volume,source=(volume name),destination=(cantainer path)' --name (name container) (image)
```
