FROM jneis/sandbox:essential

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get install -y apache2

# set vhost
COPY vhost.conf /etc/apache2/sites-enabled/000-default.conf

# set index page
COPY index.html /var/www/sandbox/index.html

# 80 - apache
EXPOSE 80

ENTRYPOINT /usr/sbin/apachectl -D FOREGROUND
