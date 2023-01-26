# Host Network

## Network

### ip a

untuk melihat ip yang kita dapatkan kita bisa menggunakan perintah:

```sh
ip a
```

### Tracepath

tracepatch berguna untuk melacak jalur yang dilalui dan melaporkan setiap lompatan di setiap jalur, ini berguna untuk mengecek jika ada koneksi yang lambat.

```sh
tracepath (dns tujuan)
```

### Ping

mengecek koneksi antara komputer kita dengan ip/dns tujuan

```sh
ping (ip/dns tujuan)
```

### routel

menampilkan perutean di ip yang kita gunakan

```sh
routel
```

### Mengambil Konten/menampilkan konten tertentu dari url

```sh
curl (link/url)
```

### Mengunduh file dari web

```sh
curl -O (link/url)
```

## Hostname

### Melihat Hostname

```sh
hostname
```

### melihat short hostname

```sh
hostname -s
```

### Mengubah Hostname

```sh
hostnamectl set-hostname (name.hostname)
```

## Mengubah Hostname dan ip dengan Gui

```sh
nmtui
```
