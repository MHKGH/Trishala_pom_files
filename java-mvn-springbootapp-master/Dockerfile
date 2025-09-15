# Runtime only (lightweight JRE)
FROM eclipse-temurin:17-jre

# Set working directory inside container
WORKDIR /app

# Copy the already built artifact from Jenkins (target folder)
COPY target/*.war app.war

# Expose port (check src/main/resources/application.properties for the correct port)
EXPOSE 8289 
# Expose port (check src/main/resources/application.properties for the correct port)
EXPOSE 8289 

# Start the application
ENTRYPOINT ["java", "-jar", "app.war"]
