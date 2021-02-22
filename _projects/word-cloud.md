---
layout: portfolio_detail
order: 12
title:  Word Cloud
name: word-cloud
badge-description: A project for generating word clouds for persian pop/rap songs and machine learning for predicting songs' genre. 
filter: filter-ai
badge-image: badge.png
category: Web, AI
client:
project-date: Spring 2018
project-url:
github-repository: abradat/WordMap
full-description: A project for generating word clouds for persian pop/rap songs and machine learning for predicting songs' genre. 
images:
    - address: 'rap.png'
      caption: 'Word Cloud for Rap Songs Collected'
    - address: 'pop.png'
      caption: 'Word Cloud for Pop Songs Collected'
    - address: 'hichkas.png'
      caption: 'Word Cloud for Hichkas, one of the most popular rappers in Iran'
---
#### Introduction
This project is implemented for **Natural Languages Processing (NLP)** course during my B.Sc. period. It has two parts:
1. For the first part, 107 pop songs and 59 rap songs' lyrics were collected from [Radio Javan](https://www.radiojavan.com/). Normalization and Tokenizing the lyrics is done by hazm python module. after normalizing and extracting the words, we store the words and how many times they were repeated in the lyrics in the artist's exclusive dictionary and category's dictionary by founding out the exact number of words repeatition, we can now have our word maps.
2. For the second part, **Deep Learning** approach was used to detect the genre (Rap/Pop) of a given lyrics as the input to the neural network.

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/python.png' | relative_url}}" width="60" height="60"> | **Python** language is used for developing the applications |
| <img src="{{'assets/img/portfolio/technologies/tensorflow.png' | relative_url}}" width="60" height="60"> | **Tensorflow** is the framework for developing machine learning applications |
| <img src="{{'assets/img/portfolio/technologies/git.png' | relative_url}}" width="60" height="60"> | **Git** is used for the version control |