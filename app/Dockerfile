FROM amazonlinux:2

RUN yum update -y
RUN amazon-linux-extras install php8.0
RUN yum install -y php php-devel php-opcache php-mbstring php-xml pdo_mysql

WORKDIR /src

EXPOSE 9000
ENTRYPOINT /usr/sbin/php-fpm -F

COPY ./www.conf /etc/php-fpm.d/www.conf
COPY ./php.ini /usr/local/etc/php/php.ini
