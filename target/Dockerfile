FROM fabric8/java-alpine-openjdk11-jre
ARG JAR_FILE=*.jar
COPY ${JAR_FILE} app.jar
ADD /application.properties application.properties
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]