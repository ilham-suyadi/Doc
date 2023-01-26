# Directory & Files

## LIst

| perintah | fungsi |
|---    |---    |
|ls     | melihat list file dan directory di dalam folder|
|ls -l  | melihat list dengan format panjang |
|ls -lh | memperihatikan ukuran file yang ada |
|ls -l --block-size=(k/m/g) | memperlihatkan ukuran file dengan format tertentu|
|ls -S | mengurutkan file dari yang terbesar |
|ls -t | mengurutkan file yang baru di edit|
|ls -X | mengurutkan file sesuai dengan ekstensi|
|ls -r | mengurutkan file dengan urutan terbalik |
|ls -R | menampilkan konten sub directori |
|ls ../| memperlihatkan isi file indux/home |
|ls ~  | menunjukkan isi dari directory home|
|ls -r |

---

## Directory

### membuat sebuah directory

```sh
mkdir (name directory)
```

### membuat beberapa directory bersamaan

```sh
mkdir (name directory 1) (name directory 2) (name directory 3)
```

### membuat directory dan menampilkan pesan proses

```sh
mkdir -v (name directory)
```

### membuat directory dan memberi akses

```sh
mkdir -m=rwx (name directory)
atau
mkdir -m 777 (name directory)
```

### membuat directory dan sub directory

```sh
mkdir -p (name directory)/(name sub directory)
```

### menghapus directory

```sh
rmdir (name directory)
```

### menghapus directory dan sub directory

```sh
mkdir -p (name directory)/(name sub directory)
```

### mengubah nama folder atau file

```sh
mv (old name) (new name)
```

### mencari sebuah sub folder

```sh
find . -depth -type d -name (New_folder)
```

---

## Membuat dan Menghapus file

### membuat file

```sh
touch (name file)
```

### menghapus file

```sh
rm (name file)
```

### menghapus file berdasarkan ekstensi

```sh
rm *(ekstensi)
```

### menghapus file secara interaktif(ada konfirmasi)

```sh
rm -i
```

### mengopy file atau directory

```sh
cp (sumber) (tujuan)
```

### mengopy directory dan sub directory

```sh
cp -r (sumber) (tujuan)
```

---

## Lain lain

### melihat posisi directory yang di akses

pwd berguna untuk me

```sh
pwd
```

### cd

```sh
cd <directory tujuan>
```
