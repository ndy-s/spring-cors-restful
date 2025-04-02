# Spring CORS Restful

A Spring Boot project demonstrating **CORS (Cross-Origin Resource Sharing)** in a RESTful API. Based on the [Spring guide](https://spring.io/guides/gs/rest-service-cors), it allows cross-origin requests using `@CrossOrigin` and handles AJAX calls from a separate frontend.

## How to Run

This project runs **two Spring Boot servers** to test CORS.

### 1. Run the Backend (Port: 8080)
```sh
./mvnw spring-boot:run
```
- API available at `http://localhost:8080/greeting`.

### 2. Run the Frontend (Port: 9000)
```sh
./mvnw spring-boot:run -Dspring-boot.run.jvmArguments='-Dserver.port=9000'
```
- Open `http://localhost:9000/index.html` to make an AJAX request to the backend.

## Reference
Based on the [Spring CORS Guide](https://spring.io/guides/gs/rest-service-cors).
