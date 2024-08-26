
# Naming Server Microservice (Eureka)

This repository contains the source code for the Naming Server Microservice of the Currency Conversion and Exchange API project. 

## Project Overview

This repository contains the Naming Server Microservice for a microservices-based application, built using Spring Boot and Eureka. The Naming Server is responsible for managing service discovery, allowing microservices to register and discover each other dynamically. It plays a crucial role in ensuring the seamless interaction between services in a distributed architecture.

## Key Features

- Centralized service registry using Eureka.
- Dynamic registration and discovery of microservices.
- Load balancing and failover capabilities.
- Dockerized deployment for scalable microservice environments.

## Technologies Used

- **Java**
- **Spring Boot**
- **Eureka Server**
- **Docker**

## Project Structure and Code Explanation

1. **Eureka Configuration**:
   - Eureka is configured as the central registry where microservices register and discover each other.
   ```yaml
   eureka:
     client:
       register-with-eureka: false
       fetch-registry: false
     server:
       enable-self-preservation: false
   ```

2. **Service Registration**:
   - Each microservice (like Currency Conversion or Currency Exchange) registers with the Eureka server for dynamic discovery.

3. **Docker Integration**:
   - Docker is used for containerizing the Eureka server, making it easy to deploy in different environments.

## Commits and Project Evolution

1. **Initial Setup**: Created the basic Eureka server configuration and Spring Boot setup.
2. **Service Registry**: Added microservice registration and service discovery features.
3. **Containerization**: Integrated Docker for deploying the Naming Server as part of the microservices architecture.

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/MalingaBandara/Naming-Server.git
   ```
2. Build the project using Maven:
   ```bash
   mvn clean install
   ```
3. Run the service:
   ```bash
   mvn spring-boot:run
   ```
4. Alternatively, use Docker to run the containerized service:
   ```bash
   docker-compose up
   ```

## Purpose and Future Enhancements

This project is designed to be a critical component of a distributed microservices architecture, demonstrating my understanding of service discovery and dynamic registration in cloud-native applications. Future enhancements may include integrating resilience mechanisms like circuit breakers and enabling secure communication using OAuth2.

## Main Repository

- [Currency Conversion and Exchange API](https://github.com/MalingaBandara/Currency-Conversion-Exchange-Microservices)

## What's Covered in This Microservice

- Implementation of service discovery using Eureka.
- Registration and discovery of microservices.
- Utilization of Docker for containerization and deployment.

## License

This project is licensed under the MIT License.
