FROM php:8.1.2-fpm

COPY php.ini /usr/local/etc/php/

RUN apt update \
  && apt install -y default-mysql-client \
  && docker-php-ext-install pdo_mysql

COPY --from=composer:2.0 /usr/bin/composer /usr/bin/composer

RUN echo 'alias la="ls -la"' >> ~/.bashrc
RUN echo 'alias ll="ls -la"' >> ~/.bashrc
RUN echo 'alias rm="rm -i"' >> ~/.bashrc
RUN echo 'alias cp="cp -i"' >> ~/.bashrc
RUN echo 'alias mv="mv -i"' >> ~/.bashrc

WORKDIR /var/www