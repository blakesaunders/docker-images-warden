ARG PHP_VERSION
FROM davidalger/warden:mage2-fpm-${PHP_VERSION}
USER root

RUN yum install -y php${PHP_VERSION}-gmp

RUN curl -sL https://dl.yarnpkg.com/rpm/yarn.repo -o /etc/yum.repos.d/yarn.repo
RUN yum install -y yarn \
    && echo 'export PATH="$HOME/.yarn/bin:$HOME/.config/yarn/global/node_modules/.bin:$PATH"' >> /home/www-data/.bashrc

USER www-data
