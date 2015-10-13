FROM jneis/sandbox:php-pecl

ENV DEBIAN_FRONTEND noninteractive

# install extension
RUN pecl install xdebug-2.2.7

# add extension to config
COPY xdebug.conf /tmp/xdebug.conf
RUN cat /tmp/xdebug.conf >>/etc/php5/apache2/php.ini || \
    rm /tmp/xdebug.conf

# 80 - apache
EXPOSE 80

ENTRYPOINT /usr/sbin/apachectl -D FOREGROUND
