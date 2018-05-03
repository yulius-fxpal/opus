FROM richarvey/nginx-php-fpm:latest

COPY . /app

RUN cd /app && \
    composer install

WORKDIR /app

CMD php artisan serve --host=0.0.0.0 --port=5000
EXPOSE 5000
