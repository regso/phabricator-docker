FROM php:7.4-fpm-buster

# required
# @see https://hub.docker.com/r/phabricator/phabricator/dockerfile
RUN apt-get update \
  && apt-get install -y --no-install-recommends
#    git \
#    imagemagick \
#    # @see https://secure.phabricator.com/w/guides/dependencies/
#    # provides ssh-keygen and ssh, these are needed to sync ssh repositories
#    openssh-client \
#    procps \
#  && rm -rf /var/lib/apt/lists/*

# php extentions
#RUN set -ex \
#  && apt-get install -y --no-install-recommends \
#    libcurl4-gnutls-dev \
#    libjpeg62-turbo-dev \
#    libpng-dev \
#    libfreetype6-dev \
#    libzip-dev \
#  && docker-php-ext-install -j "$(nproc)" \
#    gd \
#    opcache \
#    mbstring \
#    iconv \
#    mysqli \
#    curl \
#    pcntl \
#    zip

WORKDIR /var/www

CMD ["php-fpm"]