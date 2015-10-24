FROM jneis/sandbox:php

ENV DEBIAN_FRONTEND noninteractive

# download and install composer.phar
RUN curl -sS https://getcomposer.org/installer | php

# move it out the working directory
RUN mv composer.phar /usr/local/bin/composer

ENTRYPOINT /bin/bash
