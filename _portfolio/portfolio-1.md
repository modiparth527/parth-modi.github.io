---
title: "Cancer Diagnosis with Machine Learning"
excerpt: "Leveraging machine learning techniques to improve cancer diagnosis accuracy." 
collection: portfolio
---

## Problem Statement
<div style="text-align: justify;">
Cancer is a complex disease that varies significantly across individuals, making accurate diagnosis and treatment challenging. Traditional diagnostic methods often struggle to account for the intricate variations in genetic mutations and the vast amount of clinical information in medical records. This project aims to address these challenges by leveraging machine learning models to predict cancer classes using both gene variations and textual data from clinical reports, thereby improving diagnostic accuracy and assisting oncologists in early detection and personalized treatment planning.
</div>

![Cancer Diagnosis Screenshot]({{site.baseurl}}/images/1.png)
<p align="center"><em>Figure 1: Problem Statement by Oncologist</em></p>

### Sources of Problem Statement

1. [Forbes: A New Cancer Drug Helped Almost Everyone Who Took It—Almost](https://www.forbes.com/sites/matthewherper/2017/06/03/a-new-cancer-drug-helped-almost-everyone-who-took-it-almost-heres-what-it-teaches-us/#2a44ee2f6b25)
2. [YouTube: Cancer Diagnosis Techniques (Video)](https://www.youtube.com/watch?v=qxXRKVompI8)

### Buisness Constraints
* No low-latency requirement.
* Interpretability is important.
* Errors can be very costly.
* Probability of a data-point belonging to each class is needed.

## Data Set Overview

- **Source**: [Kaggle: MSK Redefining Cancer Treatment Data](https://www.kaggle.com/c/msk-redefining-cancer-treatment/data)
- We have two data files:
  - One contains information about genetic mutations.
  - The other contains clinical evidence (text) used by experts/pathologists to classify these mutations.
- Both files share a common column called **ID**.

### Data File Information:
- **training_variants**: (ID, Gene, Variations, Class)
- **training_text**: (ID, Text)

## Model Training
<div style="text-align: justify;">
 The model combines structured data (like genetic mutations) with unstructured textual information to improve classification accuracy. This involves steps like dataset preparation, feature extraction from gene, variations and text, and the application of models like BERT for text, alongside traditional machine learning methods such as SVM, decision trees, and neural networks for structured data. Performance is evaluated using standard metrics like accuracy/misclassification rate.
</div>


## Results
 
| Model                                                 | Train Log Loss | CV Log Loss | Test Log Loss | Percentage Misclassification |
|-------------------------------------------------------|----------------|-------------|---------------|------------------------------|
| Naive Bayes                                          | 0.90           | 1.27        | 1.21          | 39.84%                       |
| kNN                                                  | 0.70           | 1.13        | 1.002         | 39.47%                       |
| Logistic Regression with class balance                | 0.614          | 1.143       | 1.048         | 34.77%                       |
| Logistic Regression without class balance             | 0.628          | 1.185       | 1.054         | 36.28%                       |
| SVM                                                  | 0.739          | 1.132       | 1.063         | 36.47%                       |

*Baseline: Log loss of Random Model - 2.5*

