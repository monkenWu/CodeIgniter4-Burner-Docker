FROM webdevops/php:8.1-alpine

# php-event
RUN \
    apk add autoconf openssl-dev && apk add build-base &&\
    apk add linux-headers && apk add libevent-dev && apk add openldap-dev && apk add imagemagick-dev && \
    docker-php-ext-install opcache && docker-php-ext-enable opcache && \
    echo '' | pecl install event && \
    docker-php-ext-enable --ini-name zz-event.ini event

WORKDIR "/"