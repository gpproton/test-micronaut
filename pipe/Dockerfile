FROM openjdk:14-alpine
COPY build/libs/pipe-*-all.jar pipe.jar
EXPOSE 8080
CMD ["java", "-Dcom.sun.management.jmxremote", "-Xmx128m", "-jar", "pipe.jar"]