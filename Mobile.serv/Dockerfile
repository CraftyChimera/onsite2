FROM php:apache
COPY mobile.serv.conf /etc/apache2/sites-available/mobile.serv.conf
RUN echo "ServerName localhost" >> /etc/apache2/apache2.conf &&\a2enmod rewrite &&\a2dissite 000-default &&\a2ensite mobile.serv &&\service apache2 restart
WORKDIR /var/www/html
COPY . .
EXPOSE 8091
