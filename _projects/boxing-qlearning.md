---
layout: portfolio_detail
order: 6
title:  Boxing Q-Learning
name: boxing-qlearning
badge-description: An Agent learns how to box using Naïve Q-Learning and Deep Q Network (DQN).
filter: filter-ai
badge-image: badge-2.jpg
category: AI
client:
project-date: Fall 2017
project-url:
github-repository: abradat/boxing-qlearning
full-description: An Agent learns how to box using Naïve Q-Learning and Deep Q Network (DQN).
images:
    - address: '0-learn.png'
      caption: 'Result when 0% of learning is done.'
    - address: '50-learn.png'
      caption: 'Result when 50% of learning is done.'
    - address: '100-learn.png'
      caption: 'Result when 100% of learning is done.'
---
#### Introduction
Boxing with Q-Learning was a project for the “Artificial Intelligence” course in which an agent learns how to box using Naïve Q-Learning and Deep Q Network (DQN).

#### Technical Overview
The project is implemented by Python language with the TensorFlow framework. It is based on Reinforcement Learning and has two phases. In the first phase, implementation was done by the Naïve Q-Learning approach. Since there are many scenarios where tables are not able to scale nicely, in the second phase Deep Q Network is used. It is a deep neural network consisted of five layers: 3 Convolutional and 2 Fully-Connected Layers. With DQNs, instead of a Q Table to lookup values, there is a model that we inference (make predictions from), and rather than updating the Q table, we fit (train) your model. So, the performance and the result will be significantly enhanced. In DQN, the total number of training steps is 5000000.
<div class="text-center">
    <figure class="figure">
        <img src="{{'assets/img/portfolio/boxing-qlearning/arch.png' | relative_url}}" class="figure-img img-fluid rounded" alt="Architecture of the Network" style="width: 80%; height: 80%">
        <figcaption class="figure-caption text-center">Network architecture used for the DQN phase</figcaption>
    </figure>
</div>

#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/python.png' | relative_url}}" width="60" height="60"> | **Pytyhon** is used for implementing the application|
| <img src="{{'assets/img/portfolio/technologies/tensorflow.png' | relative_url}}" width="60" height="60"> | **Tensorflow** is the framework for implementing the Q-Learning and DQN|