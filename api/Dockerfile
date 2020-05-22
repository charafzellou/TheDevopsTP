FROM openjdk:11 AS buildstage
COPY . /usr/src/
WORKDIR /usr/src/
RUN javac Main.java

FROM openjdk:11-jre
WORKDIR /usr/src/ 
COPY --from=buildstage /usr/src/Main.class .
RUN java Main
