FROM httpd:2.4.41-alpine

RUN apk update; \
    apk upgrade;

# Copy apache vhost file to send php requests to php-fpm container
COPY apache.conf /usr/local/apache2/conf/apache.conf
RUN echo "Include /usr/local/apache2/conf/apache.conf" \
    >> /usr/local/apache2/conf/httpd.conf
