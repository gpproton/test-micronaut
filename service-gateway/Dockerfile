FROM openjdk:14-alpine
COPY build/libs/service-gateway-*-all.jar service-gateway.jar
EXPOSE 8080
CMD ["java", "-Dcom.sun.management.jmxremote", "-Xmx128m", "-jar", "service-gateway.jar"]