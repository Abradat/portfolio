---
layout: portfolio_detail_text
order: 10
title:  Microservices Patterns
name: microservices-patterns
badge-description: Implementation of microservices common patterns, including API gateway, async communication, redis sentinel, and security through OCID.
filter: filter-web
badge-image: badge.png
category: Web
client: Informatics Services Corporation (ISC)
project-date: Fall 208 - Now
project-url:
github-repository:
full-description: Implementation of microservices common patterns, including API gateway, async communication, redis sentinel, and security through OCID.
images:
    - 'direct-mapped.png'
    - 'result.png'
    - 'architecture.png'
---
#### API Gateway
API gateways are one of most important patterns in the microservices architecture which will act as the signle entry point to the system.

I have implemented API gateway based on **Netflix Zuul 1** and **Spring Cloud Gateway**. Neflix Zuul 1 is based on **blocking** flow while the Spring Cloud Gateway is implemented on Netty and is a **non-blocking** gateway that notably increases the performance.
#### Inbound API Gateway
This project is a special case of API gateway for the Iranian Instant Payment (IIP) project. It is implemented based on **Netflix** Zuul 1. The gateway exposes REST endpoints to the clinets. It receives requests and publish them to the **Apache Kafka** using Zuul filters. 

<i class="bx bxl-github"></i> Source code of the project is available from [here](https://github.com/abradat/inbound-gateway){:target="_blank"}

#### Apache Kafka/MQ Communication
In order to prevent performance decreament in microservices architecture, utilizing **asynchronous** communication besides **synchronous** communications is an essential way. I have implemented communication in microservices through **Apache Kafka** and **IBM MQ**.

<i class="bx bxl-github"></i> Apache Kafka's source code is available from [here](https://github.com/Abradat/microservice-kafka-messaging){:target="_blank"}  
<i class="bx bxl-github"></i> IBM MQ's source code is available from [here](https://github.com/Abradat/microservice-mq-messaging){:target="_blank"}

#### Redis Sentinel
Redis Sentinel provides high availability for Redis. In practical terms this means that using Sentinel you can create a Redis deployment that resists without human intervention certain kinds of failures.

I implemented Redis sentinel as a pattern for **distributed configuration** for our services. 

<i class="bx bxl-github"></i> Source code of the project is available from [here](https://github.com/abradat/redis-sentinel){:target="_blank"}

#### Security with OIDC
I implemented security pattern for microservices using **Keycloak**. It provides **OpenID Connect (OIDC)** a thin layer on the top of **OAuth2**.

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/java.png' | relative_url}}" width="60" height="60"> | **Java** is used for developing backend services |
| <img src="{{'assets/img/portfolio/technologies/spring-boot.png' | relative_url}}" width="60" height="60"> | **Spring Boot** framework is used for developing backend services based on **microservices** architecture |
| <img src="{{'assets/img/portfolio/technologies/spring.png' | relative_url}}" width="60" height="60"> | **Spring Cloud Gateway** for implementing API Gateway, **Spring Security** for security concerns, and **Spring Data JPA** for dealing with database.|
| <img src="{{'assets/img/portfolio/technologies/ibm-mq.png' | relative_url}}" width="60" height="60"> | **IBM MQ** is a message queue which is used for exchanging messages between Socket IO client and banks themselves |
| <img src="{{'assets/img/portfolio/technologies/kafka.png' | relative_url}}" width="60" height="60"> | **Apache Kafka** is a streaming platform for exchanging messages between mail and tweet servies. |
| <img src="{{'assets/img/portfolio/technologies/keycloak.png' | relative_url}}" width="60" height="60"> | **Keycloak** acts as the authentication and authorization service for the system. It is based on OpenID Connect and OAuth2 |
| <img src="{{'assets/img/portfolio/technologies/redis.png' | relative_url}}" width="60" height="60"> | **Redis** is used for implementing distributed configuration services. |
| <img src="{{'assets/img/portfolio/technologies/docker.png' | relative_url}}" width="60" height="60"> | **Docker** is used for virtualization and containerizing services, including backend and frontend services. |
| <img src="{{'assets/img/portfolio/technologies/git.png' | relative_url}}" width="60" height="60"> | **Git** is used for version control |
