FROM debian:latest
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get -y install nginx php php-mysql php-fpm php-curl php-gd php-intl php-mbstring php-soap php-xml php-xmlrpc php-zip locate nano supervisor 
WORKDIR /var/www/html
EXPOSE 80
EXPOSE 443
CMD ["/usr/bin/supervisord", "-c", "/etc/supervisor/conf.d/supervisord.conf"]
 
