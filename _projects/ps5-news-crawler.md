---
layout: portfolio_detail_large
order: 2
title:  PS5 News Crawler
name: ps5-news-crawler
badge-description: A web application for crawling the latest news from CNN and latest tweets from Twitter about PS5 console.
filter: filter-web filter-ai
badge-image: badge.jpeg
category: Web, AI
client:
project-date: December 2020
project-url:
github-repository: abradat/ps5-news
full-description: This project is web based application for crawling latest news from CNN and latest tweets and analyzing people's oponion about Sony's last gaming console, PS5.
# images:
#     - 'cnn-overall.png'
#     - 'cnn-details.png'
#     - 'twitter-overall.png'
images:
    - address: 'cnn-overall.png'
      caption: 'List of crawled news from CNN'
    - address: 'cnn-details.png'
      caption: 'Details of the news crawled from CNN'
    - address: 'twitter-overall.png'
      caption: 'List of tweets crawled from Twitter'
    - address: 'twitter-detail.png'
      caption: 'Detail of a tweet with sentiment analysis tag'
    
---
#### Introduction
This project is developed for crawling recent articles from **CNN** and recent **tweets** from people about the latest released console, PS5.

#### Components

**Spring Boot Server Application**: This application is responsible for crawling data from CNN and Twitter. Also, it exposes REST endpoints for fetching crawled data.  
**Angular Application**: The GUI web application for viewing crawled data and requesting for further crawls.  
**Selenium**: Selenium provides powerful features for web browsing automation. It is used for crawling the CNN website.  
**PostgreSQL**: This databased is used for storing crawled data from CNN and Twitter.

#### Data Crawling

1. ##### CNN Crawling
    The latest articles about PS5 is fetched from search section of CNN's website. Like many other modern websites, CNN pages are dynamic. It makes AJAX calls for receiving the latest search results. Hence, utilizing traditional parsers are not useful for crawling the search results.  
    
    Selenium can be utilized for automated crawling complex websites. it gives the user full control of the browser. For example, in crawling search results, the results will arrive after some time. So, the result elements are not available, and the user has to wait for the elements to be completely loaded. Selenium wait functions gives the user the ability to wait for some elements to load.
2. ##### Twitter Crawling
    Instead of using selenium, Twitter's Developer API is used for crawling data. Each time the latest 25 tweets containing the word PS5 are fetched from Twitter. Username, publish date, and text of the tweets are extracted from the results.

    Then, the body of tweet is analyzed by **Stanford Core NLP** for extracting the tweet's sentiment and labeling it in the GUI application. There are five possible values including, [VERY POSITIVE, POSITIVE, NEUTRAL, NEGATIVE, and VERY_NEGATIVE]. Tweet's sentiment is persisted with other fields extracted to the database.

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/java.png' | relative_url}}" width="60" height="60"> | **Java** is used for developing backend services |
| <img src="{{'assets/img/portfolio/technologies/typescript.png' | relative_url}}" width="60" height="60"> | **Typescript** is the main language used for developing Angular applications. |
| <img src="{{'assets/img/portfolio/technologies/spring-boot.png' | relative_url}}" width="60" height="60"> | **Spring Boot** framework is used for developing backend services for exposing REST endpoints and crawling CNN and Twitter |
| <img src="{{'assets/img/portfolio/technologies/spring.png' | relative_url}}" width="60" height="60"> | **Spring** frameworks, including Spring Cloud, Spring Security, Spring Data, etc. are used for developing backend services. |
| <img src="{{'assets/img/portfolio/technologies/core-nlp.png' | relative_url}}" width="120" height="60"> | **Stanford Core NLP** is used for extracting crawled tweets' sentiments in order to analyze people's oponion about PS5|
| <img src="{{'assets/img/portfolio/technologies/angular.png' | relative_url}}" width="60" height="60"> | **Angular** framework is used for developing GUI web applications. |
| <img src="{{'assets/img/portfolio/technologies/selenium.png' | relative_url}}" width="60" height="60"> | **SELENIUM** is an standalone browser for crawling CNN. |
| <img src="{{'assets/img/portfolio/technologies/docker.png' | relative_url}}" width="60" height="60"> | **Docker** is used for virtualization and containerizing services, including backend and frontend services. |
| <img src="{{'assets/img/portfolio/technologies/postgre.png' | relative_url}}" width="60" height="60"> | **PostgreSQL** databse is used for persisting news and tweets |
| <img src="{{'assets/img/portfolio/technologies/nginx.svg' | relative_url}}" width="110" height="60"> | **NGINX** web server is used for deploying angular application. |
| <img src="{{'assets/img/portfolio/technologies/git.png' | relative_url}}" width="60" height="60"> | **Git** is used for version control. |