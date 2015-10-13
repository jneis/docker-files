FROM jneis/sandbox:httpd

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get install -y php5 libapache2-mod-php5

# set new index page
RUN rm /var/www/sandbox/index.html
COPY index.php /var/www/sandbox/index.php

# 80 - apache
EXPOSE 80

ENTRYPOINT /usr/sbin/apachectl -D FOREGROUND
