FROM openjdk:17-jdk
EXPOSE 8761
ARG JAR_FILE=build/libs/*.jar
ARG RESOURCE_FILE=build/resources/main/*.yml
COPY ${JAR_FILE} app.jar
COPY ${RESOURCE_FILE} app/app.yml
CMD ["java", "-jar", "app.jar", "--spring.config.location=file:/app/app.yml"]