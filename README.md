# Nextcloud and ONLYOFFICE integrated in docker
References: [docker-onlyoffice-nextcloud] <https://github.com/ONLYOFFICE/docker-onlyoffice-nextcloud>

### Nginx config
```
curl -Lo /var/www/nginx.conf https://raw.githubusercontent.com/ONLYOFFICE/docker-onlyoffice-nextcloud/master/nginx.conf
```

### Install ONLYOFFICE
```
curl https://raw.githubusercontent.com/ONLYOFFICE/docker-onlyoffice-nextcloud/master/set_configuration.sh | sed 's/"secret"/"i4z0n3"/' | bash
```



