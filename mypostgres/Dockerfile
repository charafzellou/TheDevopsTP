FROM postgres:11.6-alpine

COPY *.sql /docker-entrypoint-initdb.d/

ENV POSTGRES_DB=db
ENV POSTGRES_USER=root
ENV POSTGRES_PASSWORD=toortoor