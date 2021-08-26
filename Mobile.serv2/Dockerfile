FROM php:apache
COPY mobile.serv2.conf /etc/apache2/sites-available/mobile.serv2.conf
RUN echo "ServerName localhost" >> /etc/apache2/apache2.conf &&\a2enmod rewrite &&\a2dissite 000-default &&\a2ensite mobile.serv2 &&\service apache2 restart
WORKDIR /var/www/html
COPY . .
EXPOSE 8093
