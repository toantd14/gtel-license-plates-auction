![Software Architecture.png](Software%20Architecture.png)

## Prerequisite
- Cài đặt JDK 17+ nếu chưa thì [cài đặt JDK](https://tayjava.vn/cai-dat-jdk-tren-macos-window-linux-ubuntu/)
- Install Maven 3.5+ nếu chưa thì [cài đặt Maven](https://tayjava.vn/cai-dat-maven-tren-macos-window-linux-ubuntu/)
- Install IntelliJ nếu chưa thì [cài đặt IntelliJ](https://tayjava.vn/cai-dat-intellij-tren-macos-va-window/)

## Technical Stacks
- Java 17
- Spring Boot 3.2.3
- PostgresSQL
- MongoDB
- ElasticSearch
- Stripe
- Kafka
- Redis
- gRPC
- Stripe
- OneSignal
- Maven 3.5+
- Lombok
- DevTools
- Docker, Docker compose
- ELK
- Grafana
- Prometheus

## Design Pattern
- Microservice Architecture
- Circuit Breaker
- Saga Pattern


## Build application
```bash
mvn clean package -P dev|test|uat|prod
```

## Run application
- Maven statement
```bash
cd account
./mvnw spring-boot:run

cd license-plates
./mvnw spring-boot:run
```
- Jar statement
```bash
cd account
java -jar target/account-service.jar

cd license-plates
java -jar target/license-plates-service.jar
```

- Docker
```bash
docker build -t cd account-service ./account
docker run -d account-service:latest account-service

docker build -t cd license-plates-service ./license-plates
docker run -d license-plates-service:latest license-plates-service
```

## Package application
```bash
docker build -t account-service ./account

docker build -t license-plates-service ./license-plates
```

