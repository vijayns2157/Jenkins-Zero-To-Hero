# Use Eclipse Temurin Java 21 base image (official and actively maintained)
FROM eclipse-temurin:21-jre-alpine

# Define the artifact path
ARG artifact=target/spring-boot-web.jar

# Set working directory
WORKDIR /opt/app

# Copy the JAR file into the container
COPY ${artifact} app.jar

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
