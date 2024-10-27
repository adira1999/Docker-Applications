# Use an official OpenJDK image as the base
FROM openjdk:17-jdk-alpine

# Set the working directory inside the container
WORKDIR /dockerApp

# Copy the JAR file from the host into the container
COPY target/docker-0.0.1-SNAPSHOT.jar myApp.jar

# Expose the application port (default for Spring Boot is 8080)
EXPOSE 2121

# Command to run the JAR file
ENTRYPOINT ["java", "-jar", "myApp.jar"]
