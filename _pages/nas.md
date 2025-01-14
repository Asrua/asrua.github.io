---
title: "Neural Architecture Search for Image Classification"
date: 2022-01-26
permalink: /nas/
author_profile: true
---


An evolutionary neural architecture search (NAS) method to automatically find deep convolutional neural network architecutures for image classification tasks on ImageNet. 

{% include toc %}

# Understand everything in 1 minute
<br />
<img align="center" width="600" src="{{ site.url }}/images/myimage/graphical_abstract.png" alt="...">
<br />

# Overview
The NAS is decoupled into two steps: weight optimization and evolutionary search. The purpose of weight optimization is to optimize the weights of a supernet which encodes the entire search space, so that we can avoid training sampled architecture from scratch (very time-consuming). The second step is to find the "good" architecutre from the search space with an evolutionary algorithm, i.e., genetic algorithm (heuristic). Mean field game is used to optimize the selection step of the genetic algorithm, which can make a good trade-off between exploration and exploitation. 

# Neural network architectures found by automatic search
<br />
<img align="center" width="600" src="{{ site.url }}/images/myimage/Search_architecture.png" alt="...">
<br />

## Hardware
* 2 NVIDIA Tesla P100 GPUs

## Software
* IDE: Visual Studio Code, SSH Host
* Programing Language: Python
* Machine Learning Framework: PyTorch
