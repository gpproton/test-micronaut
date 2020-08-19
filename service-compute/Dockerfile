FROM openjdk:14-alpine
COPY build/libs/service-compute-*-all.jar service-compute.jar
EXPOSE 8080
CMD ["java", "-Dcom.sun.management.jmxremote", "-Xmx128m", "-jar", "service-compute.jar"]