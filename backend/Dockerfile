FROM maven:3.9.9-eclipse-temurin-17
WORKDIR /app
COPY . . 
RUN mvn clean package -DskipTests
EXPOSE 8081
CMD ["java", "-jar", "/app/target/student-registration-backend-0.0.1-SNAPSHOT.jar"]

