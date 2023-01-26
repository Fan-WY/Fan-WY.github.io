---
title: "A client-edge-cloud hierarchical federated learning (FL) framework for the driving range estimation of battery electrical vehicle (BEV)"
date: 2023-01-26
permalink: /federatedLearningDRE/
author_profile: true
categories:
  - Research
  - Key Generation
tags:
  - Key Generation
  - Application
---
{% include toc %}

# Overview
FL enables devices to cooperatively train a machine learning (ML) model without sharing their private data. It has two key obstacles, however: a communication bottleneck and data heterogeneity. To overcome the communication challenge, I present a probabilistic device selection strategy that allows fewer devices to participate in training. To address the issue of data heterogeneity, we created a hierarchical FL to customize edge models for the devices.


# The hierarchical federated learning framework
<br />
<img align="center" width="600" src="{{ site.url }}/images/keygen/keygen_protocol.png" alt="...">
<br />

* Channel Probing:
  * Completed by probe request and probe response.
  * Packet Match: Because the demo is carried out in the office environment, there are many transmissions in the air from other wifi access points. The MAC address is used to filter out the useful packets.
*  Quantization: Mean and standard deviation-based quantization
*  Information Reconciliation: [BCH-based](https://github.com/jkent/python-bchlib){:target="_blank"} secure sketch
*  Privacy amplification: hash function [SHA256](https://docs.python.org/3/library/hashlib.html){:target="_blank"}
*  Randomness test: [NIST randomness test suite](https://github.com/stevenang/randomness_testsuite){:target="_blank"}

# Setup
<br />
<img align="center" width="600" src="{{ site.url }}/images/keygen/keygen_rpi_setup_photo.png" alt="...">
<br />

## Hardware
* NVIDIA GTX 1080Ti

## Software
* IDE: PyCharm
* Programing Language: Python3
* Machine Learning Framework: PyTorch
* Cloud plateform: AWS

# Prediction Results
<a href="http://www.youtube.com/watch?feature=player_embedded&v=37JyT22elm8&" target="_blank"><img src="{{ site.url }}/images/keygen/keygen_rpi_demo_screenshot.png" alt="Key Generation Demo" width="800" border="10" /></a>
