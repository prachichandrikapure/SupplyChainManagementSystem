# Use a reliable base image with Java 17
FROM eclipse-temurin:17-jdk

# Set the working directory inside the container
WORKDIR /app

# Copy the built JAR file into the container and rename it to app.jar
COPY target/eureka-server-0.0.1-SNAPSHOT.jar app.jar

# Expose the port the Eureka Server will listen on
EXPOSE 8761

# Define the container’s startup command
ENTRYPOINT ["java", "-jar", "app.jar"]
