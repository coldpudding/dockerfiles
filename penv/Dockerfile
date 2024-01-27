FROM php:7.0-alpine

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apk/repositories

RUN apk add libpng-dev libzip-dev freetype-dev \
    && docker-php-ext-configure gd --with-gd --with-freetype-dir=/usr/include/ \
    && docker-php-ext-install pdo pdo_mysql bcmath gd zip

# RUN composer config -g repo.packagist composer https://mirrors.aliyun.com/composer/
