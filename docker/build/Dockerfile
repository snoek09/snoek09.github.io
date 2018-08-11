FROM php:7-cli-alpine
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
RUN apk update && apk upgrade && \
    apk add --no-cache bash git openssh make
WORKDIR /opt
ENTRYPOINT ["make", "--makefile=docker/build/Makefile"]
CMD ["nothing"]

