# Use an official OpenJDK runtime as a parent image
FROM openjdk:17

# Set the working directory inside the container
WORKDIR /app


# Copy the packaged JAR file into the container
COPY target/inventory-service-1.0-SNAPSHOT.jar /app

# Copy application-docker.properties from src/main/resources into the container
COPY src/main/resources/application-docker.properties /app/config/

# Specify the command to run on container start
ENTRYPOINT ["java","-jar","inventory-service-1.0-SNAPSHOT.jar"]
