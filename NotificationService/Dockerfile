# Use a reliable base image with Java 17
FROM eclipse-temurin:17-jdk

# Set the working directory inside the container
WORKDIR /app

# Copy the built JAR file into the container and rename it to app.jar
COPY target/notification-service-0.0.1-SNAPSHOT.jar app.jar

# Expose the port the Notification Service will listen on
EXPOSE 8082

# Define the container’s startup command
ENTRYPOINT ["java", "-jar", "app.jar"]
