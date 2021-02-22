---
layout: portfolio_detail_large
order: 13
title:  Search Engine
name: search-engine
badge-description: A search engine based on the Inverted Index Algorithm and Flask framework.
filter: filter-web
badge-image: badge.jpg
category: Web
client:
project-date: Spring 2016
project-url:
github-repository: abradat/AP-SearchEngine
full-description: A search engine based on the Inverted Index Algorithm and Flask framework.
images:
    - address: 'search.png'
      caption: 'Basic and advance search options'
    - address: 'history.png'
      caption: 'History of the previous searches'
    - address: 'results.png'
      caption: 'Results of the searches'
---
#### Overview
This project was done for the **Advanced Programming** course during my university during Spring 2016. 

The search engine is a web application based on **Flask** framework. Data is crawled using **Scrapy** from websites containing the word "python". Crawled data is normalized by **Stanford NLTK** framework and saved to database based on **Inverted Index** Algorithm. 
#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/python.png' | relative_url}}" width="60" height="60"> | **Python** is used for developing the application. |
| <img src="{{'assets/img/portfolio/technologies/flask.png' | relative_url}}" width="80" height="60"> | **Flask** is the web framework used for this search engine. |
| <img src="{{'assets/img/portfolio/technologies/scrapy.png' | relative_url}}" width="120" height="48"> | **Scrapy** is used for crawling websites. |
| <img src="{{'assets/img/portfolio/technologies/core-nlp.png' | relative_url}}" width="110" height="60"> | **NLTK** by stanford is used for normalizing text crawled from websites.|
| <img src="{{'assets/img/portfolio/technologies/sqlite.png' | relative_url}}" width="110" height="60"> | **SQLite** is used as database|