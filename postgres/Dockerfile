FROM postgres:15.2-alpine
ARG postgres_db
ARG postgres_user
ARG postgres_password
ENV POSTGRES_DB $postgres_db
ENV POSTGRES_USER $postgres_user
ENV POSTGRES_PASSWORD $postgres_password
COPY ./schema.sql /docker-entrypoint-initdb.d/