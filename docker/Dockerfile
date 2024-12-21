FROM openjdk:8u151-jdk-alpine3.7

# Install mysql-client for mysqladmin and connection checks
RUN apk update && apk add mysql-client

EXPOSE 8070

ENV APP_HOME /usr/src/app

COPY target/shopping-cart-0.0.1-SNAPSHOT.jar $APP_HOME/app.jar

WORKDIR $APP_HOME

ENTRYPOINT exec java -jar app.jar
