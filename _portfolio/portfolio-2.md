---
title: "ECG based Atrial Fillibration Detection using AI"
excerpt: "Detect abnormal heartbeats with higher accuracy with AI <br/> <br/><img src='/parth-modi.github.io/images/AF_intro.png'>"
collection: portfolio
---

# Atrial Fibrillation Detection Using AI

## Overview
This project focuses on the application of artificial intelligence in medicine, specifically for detecting Atrial Fibrillation (AF) from single lead ECG signals. My approach utilizes deep learning techniques, including Convolutional Neural Networks (CNN), Long Short Term Memory (LSTM) and Generative Adversarial Networks (GANs), to improve the accuracy of AF detection.

## Table of Contents
- [Introduction](#introduction)
- [Methodology](#methodology)
  - [Convolutional Neural Networks (CNN)](#convolutional-neural-networks-cnn)
  - [Generative Adversarial Networks (GANs)](#generative-adversarial-networks-gans)
- [Results](#results)

## Introduction
Atrial fibrillation (AF) is the most common sustained cardiac arrhythmia, associated with increased rates of death, stroke, and heart failure. This project aims to classify ECG signals into four categories:
- Normal rhythm (N)
- AF rhythm (A)
- Other rhythm (O)
- Noisy (~)

## Methodology

### Convolutional Neural Networks (CNN)
1. **Signal Filtering**: The ECG signals were filtered to remove noise.
2. **Spectrogram Conversion**: Each ECG signal was converted into spectrograms.
3. **Training**: A 2D CNN was trained to classify the signals into the four categories.
   ![CNN Training]({{site.baseurl}}/images/CNN_result.png)
   <p align="center"><em>Figure 1: Confusion Matrix from basic CNN</em></p>
### Generative Adversarial Networks (GANs) + CNN & LSTM
To address the overfitting issue caused by class imbalances, we implemented GANs for data augmentation:
1. **Data Augmentation**: Artificial AF samples were generated to balance the dataset.
   ![Data Augmentation]({{site.baseurl}}/images/gan_heartbeats.png)
   <p align="center"><em>Figure 2:Artificially Generated Heartbeats by GANs</em></p>
2. **Heartbeat Template Extraction**: Heartbeat templates were extracted from each ECG signal to create artificial heartbeats.
3. **Training**: The augmented dataset was then used to train the CNN.
   ![GAN Training]({{site.baseurl}}/images/CNN_LSTM.png)
   <p align="center"><em>Figure 3: Confusion Matrix from CNN-LSTM network</em></p>

## Results
The results from both the CNN and GAN methods are detailed in the presentation slides. The GAN approach significantly improved the model's performance by addressing the class imbalance and reducing overfitting.
![Results]({{site.baseurl}}/images/results.png)



