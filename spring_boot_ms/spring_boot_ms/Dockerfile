FROM openjdk:8-jdk-alpine
WORKDIR /opt
ENV PORT 8080
EXPOSE 8080
COPY *.jar /opt/app.jar
ENTRYPOINT exec java $JAVA_OPT -jar app.jar
