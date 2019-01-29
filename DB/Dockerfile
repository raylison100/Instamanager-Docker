FROM mysql:5.7.19

MAINTAINER Raylison Nunes <raylison100@gmail.com>

RUN /usr/sbin/mysqld & \
      CREATE USER 'admin'@'localhost' IDENTIFIED BY '99291072';\
      grant all privileges on *.* to 'admin'@'localhost';\
      FLUSH PRIVILEGES; CREATE DATABASE instamanager;" | mysql /etc/mysql/my.cnf

CMD ["mysqld"]

EXPOSE 3306