---
layout: portfolio_detail_large
order: 3
title:  Iranian Instant Payment (IIP)
name: iip
badge-description: Iranian Instant Payment (IIP) is Central Bnak of Iran's newest payment system.
filter: filter-web
badge-image: badge-2.png
category: Web
client: Central Bank of Iran (CBI)
project-date: August 2019 - Present
project-url:
full-description: Iranian Instant Payment is Central Bnak of Iran's newest payment system.
images:
    - address: 'shn-01.png'
      caption: 'Screenshot of the terminal implemented in the Angular Application'
    - address: 'shn-02.png'
      caption: 'Screenshot of the terminal implemented in the Angular Application'
    - address: 'shn-04.png'
      caption: 'Screenshot of the live status of the services in the Angular Application'
    - address: 'shn-05.png'
      caption: 'Screenshot of the live status of the services in the Angular Application'
---
****NOTE: None of ISC's projects are open source. So, I am not able to share the code which I have written in this project.**
#### Introduction
IIP is Central Bank of Iran’s newest inter-bank payment system. IIP services are available all-around-the clock and should result in the immediate or close to immediate crediting of the Beneficiary’s account. The project is based on **microservice** architecture.

#### My Responsibilites
1. Developed a **Socket.IO** client based on Spring Boot for pre-defined communication between IIP and consumer banks. The client receives from and send messages to consumer banks using **IBM MQ** and communicates with Socket.IO server.
2. Developed a terminal for real-time communication between the **Angular** application and the server’s command line using **WebSocket** and **Xterm.js**.
3. **Netflix Zuul** gateway implementation for receving messages from clients based on REST endpoints and delivering them to destination services using **Apache Kafka**. For service discovery, **Eureka** server is used. [```[Source Code]```](https://github.com/Abradat/inbound-gateway){:target="_blank"}

#### Technologies/Languaes Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/java.png' | relative_url}}" width="60" height="60"> | **Java** is used for developing backend services |
| <img src="{{'assets/img/portfolio/technologies/typescript.png' | relative_url}}" width="60" height="60"> | **Typescript** is the main language used for developing Angular applications. |
| <img src="{{'assets/img/portfolio/technologies/spring-boot.png' | relative_url}}" width="60" height="60"> | **Spring Boot** framework is used for developing backend services based on **microservices** architecture |
| <img src="{{'assets/img/portfolio/technologies/spring.png' | relative_url}}" width="60" height="60"> | **Spring** frameworks, including Spring Cloud, Spring Security, Spring Data, etc. are used for developing backend services. |
| <img src="{{'assets/img/portfolio/technologies/socketio.png' | relative_url}}" width="60" height="60"> | **Socket IO** library is used for implementing its client for real-time communication with server |
| <img src="{{'assets/img/portfolio/technologies/ibm-mq.png' | relative_url}}" width="60" height="60"> | **IBM MQ** is a message queue which is used for exchanging messages between Socket IO client and banks themselves |
| <img src="{{'assets/img/portfolio/technologies/angular.png' | relative_url}}" width="60" height="60"> | **Angular** framework is used for developing GUI web applications. |
| <img src="{{'assets/img/portfolio/technologies/docker.png' | relative_url}}" width="60" height="60"> | **Docker** is used for virtualization and containerizing services, including backend and frontend services. |
| <img src="{{'assets/img/portfolio/technologies/svn.png' | relative_url}}" width="100" height="60"> | **SVN** is used for version control |