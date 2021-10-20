FROM ubuntu

RUN apt-det -y upadte
RUN apt-get -y install apache2

RUN echo 'Hello Worls from Docker!' > /var/www/html/index.html

CMD ["/usr/sbin/apachectl", "-DFOREGROUND"]
EXPOSE 80