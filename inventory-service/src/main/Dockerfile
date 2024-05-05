# Use an official OpenJDK runtime as a parent image
FROM openjdk:17

# Set the working directory inside the container
WORKDIR /app

# Expose port 8080 for the Spring Boot application
EXPOSE 8081


# Copy the packaged JAR file into the container
COPY target/discovery-server.jar /app/


# Copy application-docker.properties into the container
COPY config/application-docker.properties /app/config/

# Specify the command to run on container start
CMD ["java", "-jar", "/app/discovery-server.jar"]