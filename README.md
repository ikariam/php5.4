# php5.4
install php54 centos

mkdir /opt/php-5.6.30
mkdir /usr/local/src/php5-build
cd /usr/local/src/php5-build
wget http://de.php.net/get/php-5.6.30.tar.bz2/from/this/mirror -O php-5.6.30.tar.bz2
tar jxf php-5.6.30.tar.bz2

./configure or ./configure --prefix=/opt/php-5.6.30 --with-pdo-pgsql --with-zlib-dir --with-freetype-dir --enable-mbstring --with-libxml-dir=/usr --enable-soap --enable-calendar --with-curl --with-mcrypt --with-zlib --with-gd --with-pgsql --disable-rpath --enable-inline-optimization --with-bz2 --with-zlib --enable-sockets --enable-sysvsem --enable-sysvshm --enable-pcntl --enable-mbregex --enable-exif --enable-bcmath --with-mhash --enable-zip --with-pcre-regex --with-mysql --with-pdo-mysql --with-mysqli --with-jpeg-dir=/usr --with-png-dir=/usr --enable-gd-native-ttf --with-openssl --with-fpm-user=www-data --with-fpm-group=www-data --with-libdir=/lib/x86_64-linux-gnu --enable-ftp --with-imap --with-imap-ssl --with-gettext --with-xmlrpc --with-xsl --with-kerberos --enable-fpm

make
make install
