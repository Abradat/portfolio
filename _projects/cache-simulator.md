---
layout: portfolio_detail
order: 16
title:  Cache Simulator (ios)
name: cache-simulator
badge-description: an ios application for simulating caching Algorithms in CPU
filter: filter-mobile
badge-image: badge.jpeg
category: Mobile
client:
project-date: Spring 2016
project-url:
github-repository: abradat/CacheSimulator
full-description: an ios application for simulating caching Algorithms in CPU
images:
    - address: 'direct-mapped.png'
      caption: 'Direct Mapped strategy procedure'
    - address: 'result.png'
      caption: 'Result of the direct mapped strategy'
    - address: 'architecture.png'
      caption: 'Overall architecture of the application'
---
#### Introduction
Cache Simulator is a smartphone application for the **ios** platform. This project has been done for the “Computer Architecture” course, and it is used for simulating caching hit/miss process. It can simulate a cache with the following specifications:
1. 3 types of mapping: Direct Mapping, Set Associative, and Full Associative
2. 2-way, 4-way, and 8-way options for “Full Associative” and “Set Associative” mappings
3. 3 types of algorithms: LRU, FIFO, and Random
4. 4 types of address trace: art, mcf, swim, and random
5. RAM sizes: 512 KB, 1 MB, 2 MB, 4 MB, 8 MB, and 16 MB
6. Cache sizes: 1 KB, 2 KB, 4 KB, 8KB
7. Block sizes: 128 B, 256 B, 512 B, 1 KB, 2 KB

The application can simulate the caching process step by step with each combination of the above specifications, and analyze the results in a chart.  

#### Technical Overview
The application is implemented based on MVC architecture. It is consisted of 5 views which are:
1. Simulator Config View: In this view, user selects the cache specifications for simulating. Specifications are mentioned in the introduction section above.
2. Simulator Main View: This view loads when the user selects the “Simulate” button in the simulator config view, and the simulator begins the procedure. The simulation can proceed step by step if the user selects the “Next Step” button. In addition, the user is able to skip the steps and see the final result by selecting the “Run” button. Details of each step (address, block, and hit/miss result) are displayed. Also, a chart presents the hit ration every ten steps.
3. Simulator Result View: This view shows the final result of the simulation. A bar chart represents the final hit ratio, and the user can proceed to home (simulator config view) by selecting the button.
4. Documents View: This view sends a request and fetches the documentation, which is located in the Github repository of the project. After fetching the data, text and images are scaled to be fitted in for every screen.
5. About Us View: This view displays the information of the project.

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/swift.png' | relative_url}}" width="60" height="60"> | **Swift** is the languages for developing ios applications. |
| <img src="/portfolio/assets/img/portfolio/technologies/ios.png" width="60" height="60"> | The application has been devloped for the **ios** platform. |