# Can use another base image 
# But be sure to use the correct version
FROM eclipse-temurin:17-jdk-alpine

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

# Set working directory inside container
WORKDIR /app

# Copy Spring-boot jar file inside container
COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java", "-jar", "app.jar"]

