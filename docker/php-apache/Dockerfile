# Base image
FROM php:7.2.1-apache

# Create moodledata directory with write permissions 
RUN cd /var/www && \
    mkdir moodledata && \
    chown www-data:www-data moodledata 

# Run apt update and install some dependancies needed for docker-php-ext
RUN apt update && apt install -y libpng-dev libicu-dev zip unzip libxml2-dev sendmail

# Install PHP extensions
RUN docker-php-ext-install mysqli gd intl zip xmlrpc soap opcache

# # Enable mod_rewrite
# RUN a2enmod rewrite

# # Reload apache
# RUN service apache2 reload