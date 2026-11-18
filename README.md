# Simple REST API

A small Java REST API built with Spring Boot and Maven. It exposes one endpoint:

| Method | Path | Response |
| --- | --- | --- |
| `GET` | `/api/hello` | `{"message":"Hello, World!"}` |

## Requirements

- JDK 17 or newer
- Apache Maven 3.6.3 or newer

Check that Java and Maven are available:

```bash
java -version
mvn -version
```

## Compile, test, and package

From the project directory, run:

```bash
mvn clean test package
```

The runnable JAR is created at `target/simple-rest-api-1.0.0.jar`.

## Run locally

Start the application:

```bash
java -jar target/simple-rest-api-1.0.0.jar
```

It listens on port `8080`. In another terminal, call the API:

```bash
curl http://localhost:8080/api/hello
```

Expected response:

```json
{"message":"Hello, World!"}
```

Stop the server with `Ctrl+C`.