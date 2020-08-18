FROM openjdk:14-alpine
COPY build/libs/compute-*-all.jar compute.jar
EXPOSE 8080
CMD ["java", "-Dcom.sun.management.jmxremote", "-Xmx128m", "-jar", "compute.jar"]