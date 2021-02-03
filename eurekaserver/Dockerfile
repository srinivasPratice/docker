FROM openjdk:8-jdk-alpine
#RUN mkdir -p /eurekaserver
#WORKDIR /eurekaserver

#COPY . .
#RUN chmod 777 mvnw
#RUN ls -l
#
#RUN pwd
#RUN ./mvnw clean install
#RUN ls
#RUN ls eurekaserver/target/
#
##ARG JAR_FILE=target/*.jar
##COPY ${JAR_FILE} app.jar
##RUN cp target/*.jar eurekaserver-0.0.1-SNAPSHOT.jar
#EXPOSE 8761
#ENTRYPOINT ["java","-jar","eurekaserver-0.0.1-SNAPSHOT.jar"]

ADD ./target/eurekaserver-0.0.1-SNAPSHOT.jar /app/
CMD ["java", "-Xmx200m", "-jar", "/app/eurekaserver-0.0.1-SNAPSHOT.jar"]

EXPOSE 8761