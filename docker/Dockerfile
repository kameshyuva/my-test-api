FROM openjdk:8-jdk-alpine
MAINTAINER cma
COPY jar/*.jar /app.jar

ENV JAVA_OPTS=""

ENV SERVER_PORT 8080

EXPOSE ${SERVER_PORT}

ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]