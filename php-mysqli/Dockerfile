# 基礎映像檔
FROM php:7.2-fpm

# 維護者資訊 bella <bellawu0902 at gmail.com>
MAINTAINER bella bellawu0902@gmail.com

# 安裝Composer
RUN apt-get install inetutils-ping && \
    apt-get install vim

RUN docker-php-ext-install mysqli && \
    docker-php-ext-install pdo_mysql

RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && \
    php composer-setup.php --install-dir=/usr/local/bin --filename=composer && \
    php -r "unlink('composer-setup.php');"
