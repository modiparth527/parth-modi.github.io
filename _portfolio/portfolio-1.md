---
title: "Cancer Diagnosis with Machine Learning"
excerpt: "Leveraging machine learning techniques to improve cancer diagnosis accuracy."
collection: portfolio
---

This portfolio project showcases the application of machine learning algorithms to aid in cancer diagnosis. By analyzing medical data, the model can assist in early detection, improving patient outcomes. The project involves dataset preparation, feature engineering, model selection (e.g., decision trees, SVM, neural networks), and performance evaluation.


![Cancer Diagnosis Screenshot](1.png)

Key aspects include data preprocessing, training/testing, and validation processes, along with visualization of results.
 
| Model             | Train Log Loss | CV Log Loss | Test Log Loss | Percentage Misclassification |
|-------------------|----------|-----------|---------|----------|
| Naive Bayes      | 0.90      | 1.27      | 1.21    | 39.84%     |
| kNN               | 0.70      | 1.13      | 1.002    | 39.47%     |
| Logistic Regression with class balance     | 0.614     | 1.143      | 1.048    | 34.77%    |
| Logistic Regression without class balance     | 0.628      | 1.185      | 1.054    | 36.28%     |
| Gradient Boosting  | 0.739      | 1.132      | 1.063    | 36.47%     |
