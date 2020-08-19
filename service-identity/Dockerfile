FROM openjdk:14-alpine
COPY build/libs/service-identity-*-all.jar service-identity.jar
EXPOSE 8080
CMD ["java", "-Dcom.sun.management.jmxremote", "-Xmx128m", "-jar", "service-identity.jar"]