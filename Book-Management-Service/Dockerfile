FROM php:7.4-apache

WORKDIR /var/www/html

COPY . /var/www/html

COPY db/db.php /db

COPY book-management.sql /tmp/

RUN docker-php-ext-install mysqli

# RUN service apache2 start && sleep 5 && cat /tmp/book-management.sql | mysql -u root -h localhost "book-management"

EXPOSE 8080

CMD [ "apache2-foreground" ]