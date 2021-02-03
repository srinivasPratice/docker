FROM openjdk:8-jdk-alpine
#RUN mkdir -p /clienttwo
#WORKDIR /clienttwo
#COPY . .#RUN chmod 777 mvnw
#RUN ls -l
#
#RUN pwd
#RUN ./mvnw clean install
#RUN ls
#RUN ls clientone/target/
#
##ARG JAR_FILE=target/*.jar
##COPY ${JAR_FILE} app.jar
##RUN cp target/*.jar clienttwo-0.0.1-SNAPSHOT.jar
#EXPOSE 7000
#ENTRYPOINT ["java","-jar","clienttwo-0.0.1-SNAPSHOT.jar"]

ADD ./target/clienttwo-0.0.1-SNAPSHOT.jar /app/
CMD ["java", "-Xmx200m", "-jar", "/app/clienttwo-0.0.1-SNAPSHOT.jar"]

EXPOSE 7000
