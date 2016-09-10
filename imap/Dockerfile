FROM tutum/lamp:latest

RUN apt-get update && apt-get install php5-imap
RUN rm -rf /var/lib/apt/lists/*
RUN php5enmod imap

EXPOSE 80 3306
VOLUME /var/log/apache2
VOLUME /var/www/html

CMD ["/run.sh"]
