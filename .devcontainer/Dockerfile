# Use the official openjdk image to build the app
FROM openjdk:17-jdk-slim as build

# Set the working directory inside the container
WORKDIR /app

# Copy the jar file generated from the target directory
COPY target/helloworld-0.0.1-SNAPSHOT.jar /app/helloworld.jar

# Expose the port that Spring Boot will run on
EXPOSE 8080

# Command to run the Spring Boot application
ENTRYPOINT ["java", "-jar", "helloworld.jar"]
