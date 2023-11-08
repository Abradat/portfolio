---
layout: portfolio_detail_text
order: 1
title:  SAP Feature Flag Service
name: ffs
badge-description: SAP's Feature Flagging Service on HANA and Analytics product.
filter: filter-web
badge-image: badge.png
category: Web
client:
project-date: September 2022 - April 2023
full-description: Feature Flagging microservice withinn SAP's HANA and Analytics organization.
---
#### Introduction
Feature flags (also known as feature toggles or feature switches) are a software development technique that turns certain functionality on and off during runtime, without deploying new code. This allows for better control and more experimentation over the full lifecycle of features.

The idea behind feature flags is to build conditional feature branches into code in order to make logic available only to certain groups of users at a time. If the flag is “on,” new code is executed, if the flag is “off,” the code is skipped. Also referred to as or release toggles, feature flags are a best practice in DevOps, often occurring within distributed version control systems.

Feature Flagging Service (FFS) is a service within SAP's HANA and Analytics microservice architecture. I worked as an Agile Test Developer Intern on this project from September 2022 to April 2023. 

#### Responsibilities
As an Agile Test Developer Intern, I got deep into testing and automation besides feature development on the team. I got hands-on experience with best practices in the design, development, maintenance, and testing of a scalable and cloud-native enterprise software. 

As a member of the team, I:
1. Developed new **REST API**s to expose new features and control the automation of certain internal tasks within FFS using **Spring Boot (Java)** framework.
2. Created and 5 five **Jenkins** pipelines to streamline the test automation, instance backup automation, service data management, and aggregation the data from instances across all regions to generate customizable reports, resulting reduction of 2+ days of manual work to under 15 minutes. 
3. Imeplemented and performed **autommated testing** and **manual testing** at unit testing and integration testing levels using **JUnit**, **Mockito**, **PowerMock**, and utilized **Postman** for automating **API testing**.
4. Performed regular **regression testing** before new releases to ensure the stability of product before each release.
5. Employed **Jasmine** and **Mocha** tests to validate data submissions from other services to FFS.
6. Designed and integrated a **Slack bot** in **PHP**, enhancing user interaction with the FFS through Slack
6. Produced 10+ software documentation, including test plans and reports, elaborating on changes, deployment guidelines, and Slack Bot documentation.

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/java.png' | relative_url}}" width="60" height="60"> | **Java** language is used for the FFS development |
| <img src="{{'assets/img/portfolio/technologies/js.png' | relative_url}}" width="60" height="60"> | **JavaScript** is used on the Node module. |
| <img src="{{'assets/img/portfolio/technologies/groovy.png' | relative_url}}" width="60" height="60"> | **Groovy** is used in developing Jenkins pipelines' scripts. |
| <img src="{{'assets/img/portfolio/technologies/php.svg' | relative_url}}" width="60" height="60"> | **PHP** is used as a technology for developing Slack Bot. |
| <img src="{{'assets/img/portfolio/technologies/spring-boot.png' | relative_url}}" width="60" height="60"> | **Spring Boot** |
| <img src="{{'assets/img/portfolio/technologies/junit5.png' | relative_url}}" width="120" height="50"> | **JUnit** is used for unit testing on the Java module. |
| <img src="{{'assets/img/portfolio/technologies/jasmine.png' | relative_url}}" width="60" height="60"> | **Jasmine** is used for unit testing on the Node module. |
| <img src="{{'assets/img/portfolio/technologies/mocha.svg' | relative_url}}" width="60" height="60"> | **Mocha** is used for unit testing on the Node module. |
| <img src="{{'assets/img/portfolio/technologies/jenkins.png' | relative_url}}" width="60" height="60"> | **Jenkins** pipelines are used for build and automation the build, testing, and internal requirements|
| <img src="{{'assets/img/portfolio/technologies/postman.svg' | relative_url}}" width="60" height="60"> | **Postman** is used for API Testing. |
| <img src="{{'assets/img/portfolio/technologies/gerrit.png' | relative_url}}" width="60" height="60"> | **Gerrit** (based on Git) is used for version control. |