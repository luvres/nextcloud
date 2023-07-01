# Nextcloud and ONLYOFFICE integrated in docker
References: [docker-onlyoffice-nextcloud] <https://github.com/ONLYOFFICE/docker-onlyoffice-nextcloud>

### Nginx config
```
curl -Lo /var/www/nginx.conf https://raw.githubusercontent.com/luvres/nextcloud/main/nginx.conf
```

### Deploy Nextcloud stack
```
curl https://raw.githubusercontent.com/luvres/nextcloud/main/docker-compose.yaml | docker-compose -f - up -d
```

### Install ONLYOFFICE after accessing the deployed server
```
curl https://raw.githubusercontent.com/luvres/nextcloud/main/set_configuration.sh | sed 's/"secret"/"i4z0n3"/' | bash
```
