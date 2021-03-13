---
layout: portfolio_detail_large
order: 1
title:  CSD V2
name: csd-v2
date: 2021-02-10
badge-description: A new version of Central Bank of Iran’s CSD system based on microservices architecture.
filter: filter-web
badge-image: badge.jpg
category: Web
client: Central Bank of Iran
project-date: May 2020 - Present
project-url:
github-repository:
full-description: A new version of Central Bank of Iran’s CSD system. The project is based on the microservices architecture.
images:
    - address: 'home.png'
      caption: 'Home Page for the Admin Dashboard'
    - address: 'participants.png'
      caption: 'List of Participants in the System'
    - address: 'define.png'
      caption: 'Menu for Issuing Securities'
    - address: 'login.png'
      caption: 'Login Page'
---
****NOTE: None of ISC's projects are open source. So, I am not able to share the code which I have written in this project.**
#### Introduction
Development of the new version of Central Securities Depository (CSD) system of the Central Bank of Iran (CBI) started from May 2020. Business of the system completely changed. Also, we started writing code from scratch using **Spring Boot** and **Spring** frameworks for back-end development based **microservices** architecture. Also, the Web UI dashboard was completely redesigned and implemented based on **Angular** framework and **Nebular** web kit.

<div class="text-center">
    <figure class="figure">
        <img src="{{'assets/img/portfolio/csd-v2/arch.png' | relative_url}}" class="figure-img img-fluid rounded" alt="Technical Architecture">
        <figcaption class="figure-caption text-center">Technical Architecture of the System</figcaption>
    </figure>
</div>

#### My Reponsibilites
As the main developer of the team, I am responsible for:
1. Back-End services development based on **Spring Boot** and **Spring** frameworks.
2. Implemented a non-blocking API Gateway using **Spring Cloud Gateway** basted on Netty.
3. Secured services through **Keycloak** based on OpenID Connect and OAuth2.
4. Redesigned the previous Web UI and developed a new dashboard based on **Angular** framework using **Nebular** web UI kit.
5. **Dockerized** backend services and frontend application.

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/java.png' | relative_url}}" width="60" height="60"> | **Java** is used for developing backend services |
| <img src="{{'assets/img/portfolio/technologies/typescript.png' | relative_url}}" width="60" height="60"> | **Typescript** is the main language used for developing Angular applications. |
| <img src="{{'assets/img/portfolio/technologies/spring-boot.png' | relative_url}}" width="60" height="60"> | **Spring Boot** framework is used for developing backend services based on **microservices** architecture |
| <img src="{{'assets/img/portfolio/technologies/spring.png' | relative_url}}" width="60" height="60"> | **Spring** frameworks, including Spring Cloud, Spring Security, Spring Data, etc. are used for developing backend services. |
| <img src="{{'assets/img/portfolio/technologies/angular.png' | relative_url}}" width="60" height="60"> | **Angular** framework is used for developing GUI web applications. |
| <img src="{{'assets/img/portfolio/technologies/keycloak.png' | relative_url}}" width="60" height="60"> | **Keycloak** acts as the authentication and authorization service for the system. It is based on OpenID Connect and OAuth2 |
| <img src="{{'assets/img/portfolio/technologies/docker.png' | relative_url}}" width="60" height="60"> | **Docker** is used for virtualization and containerizing services, including backend and frontend services. |
| <img src="{{'assets/img/portfolio/technologies/oracledb.png' | relative_url}}" width="100" height="60"> | **Oracle** databse is used in this project. |
| <img src="{{'assets/img/portfolio/technologies/svn.png' | relative_url}}" width="100" height="60"> | **SVN** is used for version control |