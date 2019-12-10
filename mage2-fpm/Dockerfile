ARG PHP_VERSION
FROM davidalger/warden:mage2-fpm-${PHP_VERSION}
USER root

RUN yum install -y php${PHP_VERSION}-gmp

RUN curl -o- -L https://yarnpkg.com/install.sh | bash \
    && echo 'export PATH="$HOME/.yarn/bin:$HOME/.config/yarn/global/node_modules/.bin:$PATH"' >> /home/www-data/.bashrc

USER www-data
