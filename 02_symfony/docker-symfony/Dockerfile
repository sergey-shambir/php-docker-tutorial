FROM php:7.3-fpm

COPY bin /setup/bin
RUN /setup/bin/install && \
    rm -rf /setup
