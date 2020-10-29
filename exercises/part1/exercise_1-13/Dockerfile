FROM openjdk:14-jdk-alpine

WORKDIR /app

COPY ./spring-example-project-master/ ./

RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]

