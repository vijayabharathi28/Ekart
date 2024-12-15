# Use an official OpenJDK image as a base image
FROM openjdk:17-jdk-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the jar file from the host to the container
COPY target/ekart-0.0.1-SNAPSHOT.jar ekart.jar

# Expose the port the app will run on
EXPOSE 8070

# Run the Spring Boot app
ENTRYPOINT ["java", "-jar", "ekart.jar"]
