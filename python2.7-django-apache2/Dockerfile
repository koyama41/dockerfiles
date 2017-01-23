FROM koyama41/python2.7-django
MAINTAINER KOYAMA Youichi <koyama41@gmail.com>
WORKDIR /
RUN apt-get update && apt-get -y upgrade
RUN apt-get -y install apache2
RUN apt-get -y install libapache2-mod-wsgi
RUN apt-get -y install python-mysqldb