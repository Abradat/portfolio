---
layout: portfolio_detail_large
order: 4
title:  KPMG WebAR Exhibition
name: kpmg-ignition
badge-description: WebAR Application for KPMG Ignition Center's Exhibition
filter: filter-web filter-mobile
badge-image: badge.jpeg
category: Web, AR, Mobile
client: KPMG
project-date: Summer 2022
project-url: https://thecdm.ca/projects/industry-projects/mobile-augmented-reality-exhibits-kpmg-ignition
github-repository:
# full-description: The first version of Central Securities Depository system based on the microservices architecture.
images:
    - address: 'banner.webp'
      caption: 'AR Exhibition at KPMG Ignition Center'
---
#### Overview
This project is an augmented reality (AR) experience that immerses the visitors of the KPMG Ignition Centre in comprehending 17 Sustainable goals through 3D models, images, videos and physical exhibits. Using their mobile phone, the user can walk around and explore the tiles throughout the office while learning more about KPMG’s take on the SDGs.

As the main developer of the team, I was responsible for researching technologies for building web AR applications, design, implementation, and testing the application through internal and user testings. In addition, I was responsible for communication with our client regarding technologies, their limitations, and their features. 

<iframe title="vimeo-player" src="https://player.vimeo.com/video/771018271?h=ae916cbf2e" width="640" height="360" frameborder="0"    allowfullscreen></iframe>

#### Design Process
##### From Native to Mobile Application
Initially, we were planning to develop a native AR application for mobile platforms, including iOS and Android. However, our client told us that they want the app to be instantly ready-to-use, and downloading and installing an application would take a long time. Hereby, we started our research for developing a web-based AR application instead of a native mobile one. We chose <a href="https://ar-js-org.github.io/AR.js-Docs/" target="_blank">AR.js</a> library for developing the application, which is an open-source and a very light library that consumes less energy on the platforms. In addition, <a href="https://aframe.io" target="_blank">A-Frame</a> framework was chosen for rendering our 3D models and embedding them into the AR world. It also supports various features, including lighting, importing 3D models, visual inspector for debugging, etc. that we needed through our process. The whole application was developed based on the <a href="https://angular.io" target="_blank">Angular Framework</a>.
##### From Image to Barcode Markers
AR.js provides an <a href="https://ar-js-org.github.io/AR.js-Docs/image-tracking/" target="_blank">image tracking</a> feature based on <a href="https://ieeexplore.ieee.org/document/748171/" target="_blank">Natural Feature Tracking (NFT) algorithm</a>. Using this feature, we have to generate images’ features through a tool and then import them to our application. The algorithm worked really well. However, when we increased the number of images to track (up to four), the tracking accuracy started to fail. Also, we faced battery usage issues, and phones started to become hot during the tests. This was something against our goals for the project as we wanted a really easy-to-use application with lease costs. 

In addition, after increasing the number of images to track from more than five, the application was not able to track any of the tiles anymore. The feature tracking was a really resource intensive algorithm for a web application on a smartphone device. Decreasing the accuracy of the tacking could help a bit, but could not solve the problem.

After discussing the problem with our client, we started to thinking about completely alternative solutions. Then we came up with the idea of using QR codes as tracking points instead of images. We started testing standard 2D-barcode markers for AR applications. We used 3x3 markers which can supports numbers from 0 to 63. The result was impressive; we were able to track all 17 barcodes (3cm x 3cm) without having any performance and battery issues from 1-1.5m distance.

<video width="480" height="640" controls>
  <source src="/portfolio/assets/img/portfolio/kpmg-ignition/city.webm" type="video/webm">
  <source src="/portfolio/assets/img/portfolio/kpmg-ignition/city.mp4" type="video/mp4">
  <source src="/portfolio/assets/img/portfolio/kpmg-ignition/city.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
<video width="480" height="640" controls>
  <source src="/portfolio/assets/img/portfolio/kpmg-ignition/banner.webm" type="video/webm">
  <source src="/portfolio/assets/img/portfolio/kpmg-ignition/banner.mp4" type="video/mp4">
  <source src="/portfolio/assets/img/portfolio/kpmg-ignition/banner.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/typescript.png' | relative_url}}" width="60" height="60"> | **Typescript** is the main language used for developing Angular applications. |
| <img src="{{'assets/img/portfolio/technologies/arjs.png' | relative_url}}" width="80" height="60"> | **AR.js** is the open-source library used for building web-based AR applications. |
| <img src="{{'assets/img/portfolio/technologies/aframe.png' | relative_url}}" width="60" height="60"> | **A-Frame** is the framework for rendering and interacting with 3D models in an AR application. |
| <img src="{{'assets/img/portfolio/technologies/angular.png' | relative_url}}" width="60" height="60"> | **Angular** framework is used for developing GUI web applications. |