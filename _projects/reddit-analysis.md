---
layout: portfolio_detail
order: 4
title:  Reddit Analysis
name: reddit-analysis
badge-description: Application for crawling subreddit posts from the Reddit website and analyzing their parameters and trends for comparing subreddits with each other
filter: filter-ai filter-web
badge-image: logo.jpeg
category: Data crawler, Data Analysis
# client: 
project-date: Winter 2021
# project-url: https://www.notion.so/syg-lab/EcoGo-The-Green-Goblins-4b43faba1064462499d4e71fa5bf356f
github-repository: abradat/reddit-analysis
full-description: Application for crawling subreddit posts from the Reddit website and analyzing their parameters and trends for comparing subreddits with each other
images:
    - address: 'home.jpg'
      caption: 'Home Screen of the application'
    - address: 'nav.jpg'
      caption: 'Navigation screen with live tracking'
    - address: 'tree.jpg'
      caption: 'Tree house of the player'
    - address: 'tree-customize.jpg'
      caption: 'Customization screen for tree house'
    - address: 'profile.jpg'
      caption: 'Profile Screen'
    - address: 'friends.jpg'
      caption: 'Friends Section'
    - address: 'shop.jpg'
      caption: 'Shop Screen'
---
#### Introduction
This project is developed for scraping subreddit posts from [Reddit](www.reddit.com) website and analyzing the crawled data.

#### Components
* **Reddit Website Scraper**: This component is responsible for scraping reddit website, extracting defined metrics from the posts, and exporting the crawled data to a file system.
Code for this component is located under ```reddit_crawler``` directory.
* **Data Analysis**: This component takes the scraper's exported file as the input and performs analysis on the data by generating plots.
Code for this component is located under ```analysis``` directory.

#### Data Scraping
[Scrapy](https://scrapy.org/) framework is used for scraping Reddit. This powerful framework provides various features that increases the performance and gives the developer more control of the crawler.

Like many other modern websites, data is dynamically loaded in Reddit. It sends AJAX requests when user scrolls to the bottom of the page to retrieve new data from the server and then renders the new data for the user. Hence, there is no "Next Page" button for navigating between posts. This feature makes scraping the website complicated.

In order to solve this problem, requests which are sent to the server when reaching the bottom of the page can be inspected from the browser's developer tools. Reddit sends a request and asks for more posts when user reaches the bottom of the page. Server returns a json containing all the information about the new posts. UI processes the json file and renders new data for the user. These requests are used for fetching posts' data from the server.

From each post, following parameters are extracted in scrapy spider:
1. Upvote Ratio
2. Score
3. Number of Comments
4. Number of Awards
5. Created Time (timestamp)
6. Title of the Post

Then these parameters are passed through scrapy pipelines to be processed:
1. Comments and awards numbers are incremented by one in order to avoid many zeros in our dataset.
2. Sentiment of the titles are extracted using Stanford CoreNLP. It can have five values ranging from zero to four (very negative, negative, neutral, positive, and very positive). Posts' titles may give us a view about what people think about that subreddit. This feature can be useful especially in controversial topics like Xbox and Playstation.

After passing through pipelines, the processed data is then saved to a csv file.

**In this project, vim and emacs subreddits are scraped between (01-01-2021) and (01-03-2021). So, all the data analysis results are based on the data fetched from these two subreddits.**

##### Limitations
It seems that Reddit has a policy that only returns the latest 1000 posts for any subreddit. I even tried the [Old Reddit](https://old.reddit.com/) website and could not fetch more than 1000 posts. There are third-party websites like [pushshift.io](https://pushshift.io/) that provides more data. However, this project is about scraping the Reddit website.

This limitation can heavilly affect our data analysis step in many ways. For example, the latest 1000 posts' date range can vary in different subreddits. In Xbox subreddit, the 1000th post may be for maximum two weeks ago, while in Scrapy subreddit, it can be for three years ago. As a result, our extracted metrics from Xbox subreddit may not have a proper distribution like number of awards as it takes time for posts to receive awards from people. In addition, maximum 1000 posts may not be sufficient for analyzing data distribution.

#### Data Analysis
Upvote Ratio, number of comments, number of awards, created time, and score metrics are extracted from the csv file. [Scipy](https://www.scipy.org/) library is used for fitting different distributions to metrics and checking the goodness of fit based on Chi-square statistics. The most fitted distribution's parameters are extracted and used for plotting. As mentioned earlier, the distributions are affected notably by Reddit's limitation so that no distribution was fitted to the number of awards metric, because there were a limited number of posts, and older posts could not be crawled. Histogram of each metric in both subreddits and their distributions are plotted and saved.

For another type of analysis, sentiments of the titles for each subreddit are plotted in a pie chart. This chart can give us information about how people may think about the topic. For example, in controversial topics like XBOX and PS5, sentiments of the titles can tell us whether people are happy with their consoles or not.

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/python.png' | relative_url}}" width="60" height="60"> | **Flutter** framework used for developing the mobile application for iOS and Android platforms. |
| <img src="{{'assets/img/portfolio/technologies/scrapy.png' | relative_url}}" width="60" height="60"> | **Angular** framework used for developing the web application. |
| <img src="{{'assets/img/portfolio/technologies/core-nlp.png' | relative_url}}" width="60" height="60"> | **Dart** language is used for the Flutter framework |
| <img src="{{'assets/img/portfolio/technologies/scipy.png' | relative_url}}" width="60" height="60"> | **TypeScript** is the main language used for developing the Angular application. |
| <img src="{{'assets/img/portfolio/technologies/git.png' | relative_url}}" width="60" height="60"> | **Git** used as the source control.|