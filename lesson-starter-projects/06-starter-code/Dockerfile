## 1. Which base image do you want to use?
FROM maven:3.8-openjdk-17-slim
## 2. Set the working directory.
WORKDIR /app/
## 3. Copy the application's project files into the working directory.
COPY /springboot-demo .

## 4. Install the dependencies and package the application.
RUN mvn install
## 5. Document and inform the developer that the application will use the container port: 8080.
EXPOSE 8080
## 6. Define the command to run when the container starts.
CMD [ "mvn", "spring-boot:run" ]