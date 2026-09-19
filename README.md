# matchwire-backend
The backend for MatchWire

## Build, test and run

Requires JDK 21. Maven comes with the wrapper (`./mvnw`), so no local install is needed.

```bash
./mvnw -q verify          # compile and run all tests (the swarm's test command)
./mvnw test               # tests only
./mvnw spring-boot:run    # start the app on http://localhost:8080
curl localhost:8080/health   # -> {"status":"ok"}
```

To build a runnable jar: `./mvnw package`, then `java -jar target/matchwire-backend-0.0.1-SNAPSHOT.jar`.
