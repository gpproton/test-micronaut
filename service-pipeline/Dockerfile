FROM openjdk:14-alpine
COPY build/libs/service-pipeline-*-all.jar service-pipeline.jar
EXPOSE 8080
CMD ["java", "-Dcom.sun.management.jmxremote", "-Xmx128m", "-jar", "service-pipeline.jar"]