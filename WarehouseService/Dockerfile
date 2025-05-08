# Use a base image with Java 17
FROM eclipse-temurin:17-jdk

# Set working directory
WORKDIR /app

# Copy the pre-built JAR file
COPY target/warehouse-service-0.0.1-SNAPSHOT.jar app.jar

# Expose the port the app runs on
EXPOSE 8085

# Run the JAR file
ENTRYPOINT ["java", "-jar", "app.jar"]
