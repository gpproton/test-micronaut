FROM openjdk:14-alpine
COPY build/libs/service-summary-*-all.jar service-summary.jar
EXPOSE 8080
CMD ["java", "-Dcom.sun.management.jmxremote", "-Xmx128m", "-jar", "service-summary.jar"]