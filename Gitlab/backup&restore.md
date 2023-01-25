# Backup & Restore

## Backup

```sh
gitlab-backup create
```

## Restore

> 1. memberi akses pada file backup

```sh
chown git:git /var/opt/gitlab/backups/11493107454_2018_04_25_10.6.4-ce_gitlab_backup.tarsh
```

> 2. menghentikan beberapa proses di gitlab :
>
> ```sh
> sudo gitlab-ctl stop puma
>
> sudo gitlab-ctl stop sidekiq
> ```

> 3. memverifikasi status yang berjalan

```sh
sudo gitlab-ctl status
```

> 4. merestore file backup :

```sh
gitlab-backup restore BACKUP=11493107454_2018_04_25_10.6.4-ce
```

>:link: Referensi : 
> * <https://docs.gitlab.com/ee/raketasks/restore_gitlab.html>
> * <https://docs.gitlab.com/ee/raketasks/backup_gitlab.html>
