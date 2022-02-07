FROM adoptopenjdk/openjdk11:alpine-jre

ARG APP_NAME="product-app"
ARG APP_VERSION="0.0.1"
ARG JAR_FILE="/build/libs/${APP_NAME}-$APP_VERSION.jar"

COPY ${JAR_FILE} product-app.jar
ENTRYPOINT ["java","-jar", "product-app.jar"]