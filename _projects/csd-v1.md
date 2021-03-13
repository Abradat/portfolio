---
layout: portfolio_detail
order: 4
title:  CSD V1
name: csd-v1
badge-description: Central Bank of Iran's Central Securities Depository System
filter: filter-web
badge-image: badge.jpg
category: Web
client: Central Bank of Iran
project-date: August 2018 - August 2019
project-url:
github-repository:
full-description: The first version of Central Securities Depository system based on the microservices architecture.
images:
    - address: 'overall.png'
      caption: 'Overall Architecture of MP01 (CSD V1)'
    - address: 'dashboard.png'
      caption: 'Dashboad of the Angular Web Application'
---
****NOTE: None of ISC's projects are open source. So, I am not able to share the code which I have written in this project.**
#### Introduction
Central Bank of Iran’s service for providing inter-bank security market and communication with Tehran Exchange Market. The project was implemented based on microservice architecture.

<div class="text-center">
    <figure class="figure">
        <img src="{{'assets/img/portfolio/csd-v1/arch.png' | relative_url}}" class="figure-img img-fluid rounded" alt="Technical Architecture">
        <figcaption class="figure-caption text-center">Technical Architecture of the System</figcaption>
    </figure>
</div>

#### My Responsibilites
As the main developer of the team, I am responsible for:
1. Developed back-end services based on **Spring Boot** and **Spring** frameworks.
2. Developed an **Angular** application components based on material design.
3. Implemented microservice architecture patterns including:
    1. Orchestration-based Saga pattern for managing distributed transactions. [```[code]```](https://github.com/Abradat/microservice-saga)
    2. **Redis Sentinel** for automatic failover, monitoring, and notification service.
    3. **IBM MQ** messaging [```[code]```](https://github.com/Abradat/microservice-mq-messaging) and **Apache Kafka** streaming. [```[code]```](https://github.com/Abradat/microservice-kafka-messaging)

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/java.png' | relative_url}}" width="60" height="60"> | **Java** is used for developing backend services |
| <img src="{{'assets/img/portfolio/technologies/typescript.png' | relative_url}}" width="60" height="60"> | **Typescript** is the main language used for developing Angular applications. |
| <img src="{{'assets/img/portfolio/technologies/spring-boot.png' | relative_url}}" width="60" height="60"> | **Spring Boot** framework is used for developing backend services based on **microservices** architecture |
| <img src="{{'assets/img/portfolio/technologies/spring.png' | relative_url}}" width="60" height="60"> | **Spring** frameworks, including Spring Cloud, Spring Security, Spring Data, etc. are used for developing backend services. |
| <img src="{{'assets/img/portfolio/technologies/ibm-mq.png' | relative_url}}" width="60" height="60"> | **IBM MQ** is a message queue which is used for exchanging messages between Socket IO client and banks themselves |
| <img src="{{'assets/img/portfolio/technologies/angular.png' | relative_url}}" width="60" height="60"> | **Angular** framework is used for developing GUI web applications. |
| <img src="{{'assets/img/portfolio/technologies/docker.png' | relative_url}}" width="60" height="60"> | **Docker** is used for virtualization and containerizing services, including backend and frontend services. |
| <img src="{{'assets/img/portfolio/technologies/svn.png' | relative_url}}" width="100" height="60"> | **SVN** is used for version control |