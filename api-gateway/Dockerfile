# Use an official OpenJDK runtime as a parent image
FROM openjdk:17

# Set the working directory inside the container
WORKDIR /app

# Expose port 8080 for the Spring Boot application
EXPOSE 8081

# Copy the packaged JAR file into the container
COPY target/api-gateway-1.0-SNAPSHOT.jar /app

# Copy application-docker.properties from src/main/resources into the container
COPY src/main/resources/application-docker.properties /app/config/

# Specify the command to run on container start
ENTRYPOINT ["java","-jar","api-gateway-1.0-SNAPSHOT.jar"]
