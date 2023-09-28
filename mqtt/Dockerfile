FROM eclipse-mosquitto:latest

COPY ./config/ /mosquitto/config/
RUN chmod 0600 /mosquitto/config/* && \
  mosquitto_passwd -c -b /mosquitto/config/pwdfile superuser "SuperMqtt" && \
  mosquitto_passwd -b /mosquitto/config/pwdfile mysqlitto "3(9R9wM<" && \
  mosquitto_passwd -b /mosquitto/config/pwdfile device "9K1^U2fQ"

VOLUME /mosquitto/config /mosquitto/data
