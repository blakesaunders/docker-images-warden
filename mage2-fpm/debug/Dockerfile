ARG PHP_VERSION
FROM davidalger/warden:mage2-fpm-${PHP_VERSION}-debug
USER root

RUN yum install -y php${PHP_VERSION}-gmp

USER www-data
