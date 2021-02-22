---
layout: portfolio_detail
order: 7
title:  Ball Trajectory Prediction
name: ball-trajectory-predictor
badge-description: A method for prediciting a rolling ball's trajectory based on the combination of K-NN Regression and Autoregression methods.
filter: filter-robotics filter-ai
badge-image: badge.png
category: Robotics, AI
client:
project-date: Fall 2018 - Fall 2019
project-url:
github-repository: abradat/ball-trajectory-predictor
full-description: a method for prediciting a rolling ball's trajectory based on the combination of K-NN Regression and Autoregression methods.
images:
    - address: 'sim.png'
      caption: 'Setup for Gazebo Simulation Environment'
    - address: 'real-ball.png'
      caption: 'Setup for Real Environment'
---
#### Overview
Prediction of the trajectory of the moving objects is of paramount importance in different fields of intelligent systems. In this paper, we proposed a novel method for prediction of trajectory of the ball on the soccer field for the humanoid robots. Our proposed method is based on combination of the k-nearest neighbor regression and autoregression models. First, k-nearest neighbor regression is enhanced by adding a cost function, which constitutes the fixed prediction scheme. Moreover, during the movement of the ball, autoregression method coefficients are updated in fixed predefined steps in order to lessen the error of the prediction, which constitutes the adaptive prediction scheme. Our proposed method is tested by simulation and practical implementation. The results demonstrate a high precision rate, in addition to the effectiveness of the adaptive scheme in case of applying external disturbance on the ball trajectory.

#### Publication
The results of this work has been published as a conference paper in ICROM 2019. The full-text version of the paper is available through [here](https://www.researchgate.net/publication/336798460_Ball_Trajectory_Prediction_for_Humanoid_Robots_Combination_of_k-NN_Regression_and_Autoregression_Methods)

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/python.png' | relative_url}}" width="60" height="60"> | **Python** language is for implementing trajectory predictor code. |
| <img src="{{'assets/img/portfolio/technologies/cpp.png' | relative_url}}" width="60" height="65"> | **C++** is used for writing scripts in ROS framework and Gazebo simulator. |
| <img src="{{'assets/img/portfolio/technologies/ros.png' | relative_url}}" width="120" height="40"> | **ROS** is the framework for running robot code and connecting to Gazebo. |
| <img src="{{'assets/img/portfolio/technologies/gazebo.png' | relative_url}}" width="60" height="60"> | **Gazebo** is the simulator used for testing our simulations. |