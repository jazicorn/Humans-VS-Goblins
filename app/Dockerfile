FROM adoptopenjdk/openjdk11:alpine-jre

ARG APP_NAME="app"
ARG JAR_FILE="/build/libs/${APP_NAME}.jar"

COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar", "app.jar"]