# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM eclipse-temurin:17-jdk-alpine

# Set the artifact path
ARG artifact=target/spring-boot-web.jar

# Create and set working directory
WORKDIR /opt/app

# Copy the built jar file into the image
COPY ${artifact} app.jar

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]

CMD ["tail", "-f", "/dev/null"]

