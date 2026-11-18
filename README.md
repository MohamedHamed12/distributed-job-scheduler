# Distributed Job Scheduler

A distributed job scheduling system built incrementally with Java, Spring Boot, PostgreSQL, and later Go workers.

## Current stage

Bootstrap only. The application is intentionally a single Spring Boot service backed by PostgreSQL. Scheduler logic, retries, distributed workers, Kafka, and Redis are not implemented yet.

## Stack

- Java 25
- Spring Boot 4.1.2
- Maven
- PostgreSQL
- Flyway
- Testcontainers

## Prerequisites

- Java 25
- Maven 3.6.3+
- Docker with Docker Compose

## Run PostgreSQL

```bash
docker compose up -d
```

## Run the application

```bash
mvn spring-boot:run
```

## Run tests

```bash
mvn test
```

The Spring context test starts PostgreSQL with Testcontainers, so Docker must be available.
