FROM mysql:latest

ENV MYSQL_ROOT_PASSWORD=m@sterkey
ENV TZ=Europe/Moscow

COPY ./sql/ /docker-entrypoint-initdb.d/

VOLUME /var/lib/mysql

CMD ["mysqld", "--default-authentication-plugin=mysql_native_password"]
