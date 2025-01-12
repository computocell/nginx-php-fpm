[![Docker Hub; wyveo/nginx-php-fpm](https://img.shields.io/badge/docker%20hub-wyveo%2Fnginx--php--fpm-blue.svg?&logo=docker&style=for-the-badge)](https://hub.docker.com/r/wyveo/nginx-php-fpm/) [![](https://img.shields.io/microbadger/image-size/wyveo/nginx-php-fpm/php70.svg?&style=for-the-badge)](https://microbadger.com/images/wyveo/nginx-php-fpm) [![](https://img.shields.io/microbadger/layers/wyveo/nginx-php-fpm/php70.svg?&style=for-the-badge)](https://microbadger.com/images/wyveo/nginx-php-fpm) [![nginx 1.17.2](https://img.shields.io/badge/nginx-1.17.2-brightgreen.svg?&logo=nginx&logoColor=white&style=for-the-badge)](https://nginx.org/en/CHANGES) [![php 7.0.33](https://img.shields.io/badge/php--fpm-7.0.33-blue.svg?&logo=php&logoColor=white&style=for-the-badge)](https://secure.php.net/releases/7_0_33.php) [![License MIT](https://img.shields.io/badge/license-MIT-blue.svg?&style=for-the-badge)](https://github.com/wyveo/nginx-php-fpm/blob/master/LICENSE)
## Introdução
Este é um Dockerfile para construir uma imagem de contêiner baseada no debian executando o nginx e o php-fpm 7.3.x / 7.2.x / 7.1.x / 7.0.x & Composer

### Versioning
| Docker Tag | GitHub Release | Nginx Version | PHP Version | Debian Version |
|-----|-------|-----|--------|--------|
| latest | master Branch |1.17.2 | 7.3.8 | buster |
| php73 | php73 Branch |1.17.2 | 7.3.8 | buster |
| php72 | php72 Branch |1.17.2 | 7.2.21 | buster |
| php71 | php71 Branch |1.17.2 | 7.1.31 | buster |
| php70 | php70 Branch |1.17.2 | 7.0.33 | buster |
## Building from source
To build from source you need to clone the git repo and run docker build:
```
$ git clone https://github.com/wyveo/nginx-php-fpm.git
```

followed by
```
$ docker build -t nginx-php-fpm:php70 . # PHP 7.0.x
```


## Pulling from Docker Hub
```
$ docker pull wyveo/nginx-php-fpm:php70
```

## Running
To run the container:
```
$ sudo docker run -d wyveo/nginx-php-fpm:php70
```

Default web root:
```
/usr/share/nginx/html
```
