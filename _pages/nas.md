---
title: "Neural Architecture Search for Image Classification"
date: 2022-10-12
permalink: /nas/
author_profile: true
categories:
  - Research
  - Key Generation
tags:
  - Key Generation
  - Application
---


An evolutionary neural architecture search (NAS) method to automatically find deep convolutional neural network architecutures for image classification tasks on ImageNet. 

{% include toc %}

# Understand everything in 1 minute
<br />
<img align="center" width="600" src="{{ site.url }}/images/myimage/graphical_abstract.png" alt="...">
<br />

# Overview
The NAS is decoupled into two steps: weight optimization and evolutionary search. The purpose of weight optimization is to optimize the weights of a supernet which encodes the entire search space, so that we can avoid training sampled architecture from scratch (very time-consuming). The second step is to find the "good" architecutre from the search space with an evolutionary algorithm, i.e., genetic algorithm (heuristic). Mean field game is used to optimize the selection step of the genetic algorithm, which can make a good trade-off between exploration and exploitation. 

# Search Result
<br />
<img align="center" width="600" src="{{ site.url }}/images/myimage/Search_architecture.png" alt="...">
<br />

## Hardware
* 2 NVIDIA Tesla P100 GPUs

## Software
* Visual Studio Code, SSH Host
* Programing Language: Python
* Machine Learning Framework: PyTorch

[commnet]: <> # Demo Video
[comment]: <a href="http://www.youtube.com/watch?feature=player_embedded&v=QXeVH1ViXXw&" target="_blank"><img src="{{ site.url }}/images/keygen/keygendemo_screenshot.png" alt="Key Generation Demo" width="800" border="10" /></a>

[comment]: # Acknowledgement
[comment]: We would like to thank [Mango Communications](http://mangocomm.com/){:target="_blank"} for their technical support on WARP and  Mr Yan Wang for his hard work on completing this excellent demo. 


[comment]: <a href="http://www.youtube.com/watch?feature=player_embedded&v=zcCXj5M2x0k&" target="_blank"><img src="{{ site.url }}/images/keygen/keygendemo_screenshot.png" alt="Key Generation Demo" width="1000" border="10" /></a>

[comment]: <><iframe width="560" height="315" src="http://www.youtube.com/embed/zcCXj5M2x0k" frameborder="0"> </iframe>
