FROM openjdk:17

ARG JAR_FILE=target/*.jar

COPY ${JAR_FILE} auction-service.jar

ENTRYPOINT ["java", "-jar", "auction-service.jar"]

EXPOSE 8083