# docker-lamp

Basic PHP/Apache/MariaDB setup to do whatever



```
cd /var/www
mkdir moodledata
chown www-data:www-data moodledata 
```

```
apt update && apt install -y libpng-dev libicu-dev zip unzip libxml2-dev sendmail
docker-php-ext-install mysqli gd intl zip xmlrpc soap opcache
service apache2 reload
```