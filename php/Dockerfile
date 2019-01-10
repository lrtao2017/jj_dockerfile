# yum install php7.2
# 20190109

FROM centos7.5:nginx_last

MAINTAINER lrtao2010@163.com


#安装yum源
RUN rpm -Uvh https://mirror.webtatic.com/yum/el7/epel-release.rpm
RUN rpm -Uvh https://mirror.webtatic.com/yum/el7/webtatic-release.rpm

#yum 安装php-7.2
RUN yum install php72w php72w-bcmath php72w-cli php72w-common php72w-dba php72w-devel php72w-embedded php72w-enchant php72w-fpm php72w-gd php72w-imap php72w-interbase php72w-intl php72w-ldap php72w-mbstring php72w-mcrypt php72w-mssql php72w-mysqlnd php72w-odbc php72w-opcache php72w-pdo php72w-pear.noarch php72w-pecl-apcu php72w-pecl-apcu-devel php72w-pecl-gearman php72w-pecl-geoip php72w-pecl-igbinary php72w-pecl-igbinary-devel php72w-pecl-imagick php72w-pecl-imagick-devel php72w-pecl-memcache php72w-pecl-memcached php72w-pecl-redis php72w-pecl-xdebug php72w-pgsql php72w-phpdbg php72w-process php72w-pspell php72w-recode php72w-snmp php72w-soap php72w-tidy php72w-xml php72w-xmlrpc -y

#启动php和nginx
CMD /usr/sbin/php-fpm && /usr/sbin/nginx -c /etc/nginx/nginx.conf


