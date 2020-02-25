FROM lynix757/centos-7

RUN yum --enablerepo=remi-php73 -y install php \
                                           php-fpm \
                                           php-bcmath \
                                           php-cli \
                                           php-common \
                                           php-gd \
                                           php-intl \
                                           php-ldap \
                                           php-mbstring \
                                           php-mysqlnd \
                                           php-pear \
                                           php-soap \
                                           php-xml \
                                           php-xmlrpc \
                                           php-json \
                                           php-mcrypt\
                                           php-zip \
                                           php-gmp \
                                           php-enchant \
                                           php-pecl-igbinary \
                                           php-odbc \
                                           php-oci8 \
                                           php-pgsql \
                                           php-pecl-amqp \
                                           php-pecl-apcu \
                                           php-pecl-msgpack \
                                           php-pecl-oci8 \
                                           php-pecl-redis5
RUN yum clean all && \
    rm -rf /var/cache/yum