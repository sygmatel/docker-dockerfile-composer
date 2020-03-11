# Extend composer container
FROM composer:1.6
MAINTAINER Charlie Henaff <c.henaff@sygmatel.fr>

RUN docker-php-ext-configure gd \ 
  && docker-php-ext-configure ldap --with-libdir=lib/x86_64-linux-gnu \
  && docker-php-ext-install \
    gd ldap json
