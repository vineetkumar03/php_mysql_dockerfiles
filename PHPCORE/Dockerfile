From  vineetkumar03/php:7.4-alpine
LABEL maintainer="vineet.wsd@nic.in"

ADD src /app/public

ENV MYSQL_HOST localhost
ENV MYSQL_USERNAME tests
ENV MYSQL_PASSWORD tests
ENV MYSQL_DATABASE register

RUN chown -R www-data:www-data /app
