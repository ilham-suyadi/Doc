# Menginstal docker di centos

## Menghapus Versi lama dari docker

```sh
yum remove docker \
             docker-client \
             docker-client-latest \
             docker-common \
             docker-latest \
             docker-latest-logrotate \
             docker-logrotate \
             docker-engine
```

## Menginstall docker mengunakan repository

### Add Repository

```sh
yum install -y yum-utils
```

```sh
yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo
```

### Install Docker

```sh
yum install docker-ce docker-ce-cli containerd.io docker-compose-plugin
```

### Memulai Docker

```sh
systemctl start docker
```

### Memverifikasi docker

```sh
docker run hello-world
```

> :link: Referensi : <https://docs.docker.com/engine/install/centos/>
