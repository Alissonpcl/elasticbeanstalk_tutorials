FROM ubuntu
COPY ./app.zip /app/app.zip
WORKDIR /app
RUN apt-get update && apt-get install unzip
RUN unzip app.zip -d ./

FROM openjdk:13
COPY --from=0 /app/play-java-hello-world-tutorial-1.0-SNAPSHOT/ /app
WORKDIR /app/bin
EXPOSE 9000
CMD ["./play-java-hello-world-tutorial", "-Dplay.http.secret.key=secret_test"]