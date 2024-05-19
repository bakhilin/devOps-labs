FROM maven:3.6.3-openjdk-11-slim 
WORKDIR /app
COPY .  /app/
RUN mvn clean install
RUN mvn package
CMD ["java", "-jar", "target/hobbie-backend-0.0.1-SNAPSHOT.jar"]

RUN rm -rf /var/cache/apk/*

