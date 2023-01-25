# Menginstal Gitlab di Docker

## Mengatur Volume Location

```sh
export GITLAB_HOME=(location tujuan)
atau
export GITLAB_HOME=/srv/gitlab
```

## Menginstal Gitlab Menggunakan Docker Compose

> 1. membuat ***docker-compose.yml*** yang berisi:

```sh
    version: '3.6'

    services:
    web:
        image: 'gitlab/gitlab-ee:latest'
        restart: always
        hostname: 'gitlab.example.com'
        environment:
        GITLAB_OMNIBUS_CONFIG: |
            external_url 'https://gitlab.example.com'
        ports:
        - '80:80'
        - '443:443'
        - '22:22'
        volumes:
        - '$GITLAB_HOME/config:/etc/gitlab'
        - '$GITLAB_HOME/logs:/var/log/gitlab'
        - '$GITLAB_HOME/data:/var/opt/gitlab'
        shm_size: '256m'
```

</br>

> 2. menjalankan docker compose dengan perintah:

```sh
docker compose up -d
```

> > :link: Referensi : <https://docs.gitlab.com/ee/install/docker.html>
