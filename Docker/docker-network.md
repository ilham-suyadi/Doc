# Docker Network

| printah | fungsi |
|--- | --- |
|docker network ls | melihat Daftar Docker Network|
|docker network create (name network) |Membuat docker network Baru |
|docker network rm (name network) |menghapus docker network|
|docker inspect (name network)| Melihat Detail dari network|
|docker container run -d --name (name container) --network (name network) (image) | menambahkan network di container|
|docker volume ls|melihat volume|
|docker volume create (name volume)|membuat docker volume|
|docker volume rm (name volume)|menghapus docker volume|
|docker container run -d --mount 'type=volume,source=(volume name),destination=(cantainer path)' --name (name container) (image)|menghubungkan container dengan volume|

> :memo: saat menghapus volume pastikan volume tidak di gunakan container
