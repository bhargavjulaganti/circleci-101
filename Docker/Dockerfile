FROM docker pull centos/php-71-centos7:7.1

RUN yum clean all

RUN yum install -y openssl-dev epel-release php-pear php-devel php-libsodium gd gd-devel php-gd

RUN pecl install mongodb

# install libsodium, mongodb gd
RUN echo "extension=mongodb.so" >> /etc/php.ini
RUN echo 'date.timezone="America/Detroit"' >> /etc/php.ini
