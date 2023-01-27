# Docker Container

| Perintah | Fungsi |
|--- | --- |
| docker run (name image) | docker run berguna untuk untuk membuat dan menjalankan sebuah container yang berasal dari docker image|
| docker run -d (name image) | untuk Menjalankan Docker Run di latar belakang |
|docker run --name (name container) (name image)| Mengatur Nama untuk Docker Container|
|docker run -p (port yang kita inginkan):(port dari aplikasi) (name image)| Mempublish Port Docker container|
|docker start (name container/id container) | menjalankan docker container|
|docker rm (name container/id container)| mengahpus docker container|
|docker rm $(docker ps -a -q -f status=exited)|Menghapus semua container yang berstatus exit|
|docker container prune | membersihkan docker|
|docker push (name image) | menambahkan docker image ke dalam docker local |
|docker push (name image):(versi)| mengepush docker image dengan versi tertentu|
|docker rmi (name image)|Menghapus docker image|

> :memo: catatan: untuk menghapus docker image pastikan docker image tidak di gunakan oleh container
