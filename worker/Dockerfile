FROM maven AS builder
ADD . /app
WORKDIR /app
RUN mvn dependency:resolve
RUN mvn package

FROM openjdk:21
COPY --from=builder /app /app
WORKDIR /app/target
CMD ["java", "-jar", "worker-jar-with-dependencies.jar"]
