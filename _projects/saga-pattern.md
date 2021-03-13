---
layout: portfolio_detail_large
order: 8
title:  Microservices Saga Pattern
name: saga-pattern
badge-description: Saga is a pattern for managing distributed transactions in microservices architecture.
filter: filter-web
badge-image: badge.jpg
category: Web
client:
project-date: Winter 2018
project-url:
github-repository: abradat/microservices-saga
full-description: Saga is a pattern for managing distributed transactions in microservices.
images:
    - address: 'saga.png'
      caption: 'Hexagonal Architecture of the project consitsted of Mail and Tweet services, their components and communications'
---
#### Introduction
One of the main concerns in the microservices architecture is distributed transaction management because a single transaction from user can span across various services. It gets more complicated when the transaction fails and it should be rolled back in all the previous engaged services. One of the patterns which has been introduced for solving this concern is named **Saga**.

This project is a sample of the Saga pattern which I implemented for my colleages at ISC in order to give them a better picture of distributed transaction management in microservices architecture.

#### Technical Overview
In this project a distributed transaction takes place between two services named tweet and mail. An action in tweet service needs to be confirmed by the mail service. If mail service does not confirm the action, the compensation transaction begins. Two services talk to each other using **Apache Kafka** and use a **MySQL** database. They both provide REST API, and **Docker** is used for virtualizing two services and the database. The hexagonal architecture of the project is presented in the slider above.

#### Languages/Technologies Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/java.png' | relative_url}}" width="60" height="60"> | **Java** is used for developing backend services |
| <img src="{{'assets/img/portfolio/technologies/spring-boot.png' | relative_url}}" width="60" height="60"> | **Spring Boot** framework is used for developing backend services based on **microservices** architecture |
| <img src="{{'assets/img/portfolio/technologies/spring.png' | relative_url}}" width="60" height="60"> | **Spring** frameworks, including Spring Cloud, Spring Data, etc. are used for developing backend services. |
| <img src="{{'assets/img/portfolio/technologies/kafka.png' | relative_url}}" width="60" height="60"> | **Apache Kafka** is a streaming platform for exchanging messages between mail and tweet servies. |
| <img src="{{'assets/img/portfolio/technologies/docker.png' | relative_url}}" width="60" height="60"> | **Docker** is used for virtualization and containerizing services, including backend and frontend services. |
| <img src="{{'assets/img/portfolio/technologies/git.png' | relative_url}}" width="60" height="60"> | **Git** is used for version control |