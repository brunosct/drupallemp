FROM debian:12

RUN apt update && apt install -y php-fpm
RUN apt install -y php8.2-mysql php-xml php-gd  php-json php-curl php-mbstring

RUN touch /var/log/php8.2-fpm.log && chmod a+w /var/log/php8.2-fpm.log

EXPOSE 9000

ENTRYPOINT [ "php-fpm8.2", "-F" ]