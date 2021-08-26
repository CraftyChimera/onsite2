FROM php:apache
COPY desktop.load.conf /etc/apache2/sites-available/desktop.load.conf
RUN echo "ServerName localhost" >> /etc/apache2/apache2.conf &&\a2enmod rewrite &&\a2dissite 000-default &&\a2ensite desktop.load &&\a2enmod proxy_balancer &&\a2enmod lbmethod_byrequests &&\a2enmod proxy &&\service apache2 restart
EXPOSE 8089
