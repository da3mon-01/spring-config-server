FROM davidcaste/alpine-java-unlimited-jce:latest
VOLUME /tmp
ADD spring-config-server-0.0.1-SNAPSHOT.jar app.jar
RUN sh -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]