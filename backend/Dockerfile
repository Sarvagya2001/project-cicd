# Use an official OpenJDK runtime as a parent image
FROM openjdk:11

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . .

# Build the Spring Boot application
RUN ./mvnw clean install

# Expose port 8080
EXPOSE 8080

# Run the application
CMD ["java", "-jar", "target/your-spring-boot-app.jar"]
