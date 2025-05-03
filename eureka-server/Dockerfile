# Use an official OpenJDK runtime as a base image
FROM openjdk:17-jdk-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the Maven build files and source code
COPY pom.xml ./
COPY src ./src
COPY mvnw ./
COPY .mvn ./.mvn

# Build the application
RUN ./mvnw clean package -DskipTests

# Expose the port Eureka Server runs on
EXPOSE 8761

# Command to run the application
CMD ["java", "-jar", "target/eureka-server-0.0.1-SNAPSHOT.jar"]