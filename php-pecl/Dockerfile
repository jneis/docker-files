FROM jneis/sandbox:php

ENV DEBIAN_FRONTEND noninteractive

# c compiler for pecl extensions
# curl lib for pear extensions
# pecl/pear extension libs
# php libs for pecl/pear extensions
RUN apt-get install -y \
    build-essential \
    libcurl3-openssl-dev \
    php-pear \
    php5-dev

ENTRYPOINT /bin/bash
