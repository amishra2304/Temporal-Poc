

# Temporal-Poc

## Overview
This project is a proof of concept (POC) for integrating Temporal with a Spring Boot application. It demonstrates how to use Temporal workflows and activities to manage complex business processes.

## Prerequisites
- Java 17+
- Maven 3.8+
- Docker and Docker Compose

## Running the Application
1. Build the project:
   ```bash
   mvn clean install
   ```
2. Start the application using Docker Compose:
   ```bash
   docker-compose up
   ```
## Push the start button and wait for the services to initialize.
## Accessing the Application

### Temporal UI
The Temporal UI can be accessed at:
- **URL**: [http://localhost:8088](http://localhost:8088)

### Swagger UI
The Swagger UI for the Spring Boot application can be accessed at:
- **URL**: [http://localhost:9191/swagger-ui/index.html#/travel-workflow-controller/bookTravel](http://localhost:9191/swagger-ui/index.html#/travel-workflow-controller/bookTravel)

You can use Swagger to explore and test the available REST APIs.

## Docker Details
This project uses Docker Compose to manage the application and its dependencies. The `docker-compose.yml` file includes the following services:
- **Temporal Server**: Runs the Temporal backend.
- **Application Service**: Runs the Spring Boot application.

To stop the services, run:
```bash
docker-compose down
```

## Additional Notes
- Ensure that the required ports (9191, 8088) are not in use before starting the application.
- For more information on Temporal, visit the [official documentation](https://docs.temporal.io/).
```
