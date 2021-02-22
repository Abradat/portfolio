---
layout: portfolio_detail
order: 5
title:  Coco (Unity Game)
name: coco
badge-description: A puzzle game made with Unity with Image processing for interaction.
filter: filter-ai filter-unity
badge-image: badge.png
category: Unity, AI
client:
project-date: January 2020
project-url:
github-repository: abradat/coco-unity
full-description: Coco is a unity game 
images:
    - address: '1.png'
      caption: 'Main game screen. Matched words "EDIT" and "TIDE"'
    - address: '2.png'
      caption: 'Main game screen. Matched word "EDIT".'
    - address: '3.png'
      caption: ''
    - address: '4.png'
      caption: ''
    - address: '5.png'
      caption: ''
    - address: '6.png'
      caption: ''
---
#### Introduction
Coco is a 2D puzzle game that is focused on **Human-Computer Interaction (HCI)** and guessing words by connecting letters together. The player can interact with the game either by matching the letters via mouse (or touch screen) or using pre-defined hand gestures that are recognized by the **image processing** algorithm. It is the combination of the final projects for the courses “Design of Computer Games” and “Foundation of Computer Vision.”
#### Functionality Overview
The Unity game engine is used for developing the game by C# language. The game is based on the MVP pattern. Levels are automatically constructed from words that have been placed in a file. The image processing application is written in Python language and utilizes the OpenCV framework. The game and the image processing application communicate using Socket. The game has a purchase feature for buying hazelnuts. Hazelnuts are used for receiving help from the game. If the player presses the “help” button in the game scene, one word is guessed for the player, and three hazelnuts are reduced.
<div class="text-center">
    <img src="{{'assets/img/portfolio/coco/arch.png' | relative_url}}"> 
</div>

If the player chooses to interact with the game with hand gesture recognition, the game acts as a client and receives data from the image processing application (server) whenever it detects a valid hand gesture. The player can show zero to five fingers to the camera. Finger numbers one to five are related to the location of the letters on the circle (for example in FIGURE 1, location of the letters ‘T,’ ‘I,’ ‘E,’ and ‘D’ are 1, 2, 3, and 4, respectively), and zero is used for checking the correctness of matched letters. 

If the player chooses to interact with the game by mouse (or touch screen), the game follows location of the cursor since the player clicks the mouse’s button and draws a line, recognizes the collisions between the cursor and characters, and finally builds a word by concatenating the selected letters and checks whether the result word is true or not.

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/python.png' | relative_url}}" width="60" height="60"> | **Python** is used for implementing image processing application |
| <img src="{{'assets/img/portfolio/technologies/csharp.png' | relative_url}}" width="60" height="60"> | **C#** is used in unity engine |
| <img src="{{'assets/img/portfolio/technologies/unity.png' | relative_url}}" width="60" height="60"> | **Unity** is the engine used for creating the game |
| <img src="{{'assets/img/portfolio/technologies/opencv.png' | relative_url}}" width="60" height="70"> | **OpenCV** framework is used for implementing the image processing algorithm |
| <img src="{{'assets/img/portfolio/technologies/git.png' | relative_url}}" width="60" height="60"> | **Git** is used for version control |