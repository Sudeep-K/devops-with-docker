FROM amazoncorretto:8u412-al2023-jre

COPY . .

RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
