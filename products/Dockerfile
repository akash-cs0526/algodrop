# Step 1: Use a lightweight JDK runtime image
FROM eclipse-temurin:17-jre-alpine

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy the executable jar from your host to the container
# We ignore .original and other folders to keep the image slim
COPY target/algodrop.jar app.jar

# Step 4: Expose the port your application runs on (default for Spring is 8080)
EXPOSE 8080

# Step 5: Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
