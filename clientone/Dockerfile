FROM openjdk:8-jdk-alpine
#RUN mkdir -p /clientone
#WORKDIR /clientone
#COPY . .
#RUN chmod 777 mvnw
#RUN ls -l
#
#RUN pwd
#RUN ./mvnw clean install
#RUN ls
#RUN ls clientone/target/
#
##ARG JAR_FILE=target/*.jar
##COPY ${JAR_FILE} app.jar
##RUN cp target/*.jar clientone-0.0.1-SNAPSHOT.jar
#EXPOSE 7001
#ENTRYPOINT ["java","-jar","clientone-0.0.1-SNAPSHOT.jar"]

ADD ./target/clientone-0.0.1-SNAPSHOT.jar /app/
CMD ["java", "-Xmx200m", "-jar", "/app/clientone-0.0.1-SNAPSHOT.jar"]

EXPOSE 6000
