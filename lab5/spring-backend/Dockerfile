FROM maven:3.6.3-openjdk-11-slim 
WORKDIR /app
COPY .  /app/
RUN mvn clean install
RUN mvn package
CMD ["java", "-jar", "target/hobbie-backend-0.0.1-SNAPSHOT.jar"]

RUN rm -rf /var/cache/apk/*


# FROM adoptopenjdk/openjdk11:alpine-jre  
# WORKDIR /backend
# RUN apk add git 
# RUN apk add maven 
# RUN git clone https://github.com/KotDimos/React-Spring-App-DevOps.git  
# RUN cd React-Spring-App-DevOps/spring-backend 
# RUN mvn package
    
# # # ARG JAR_FILE=target/hobbie-backend-0.0.1-SNAPSHOT.jar  
# # WORKDIR /opt/app  
# # COPY ${JAR_FILE} app.jar  
# ENTRYPOINT ["java","-jar","/target/hobbie-backend-0.0.1-SNAPSHOT.jar"]  

# RUN rm -rf /var/cache/apk/*