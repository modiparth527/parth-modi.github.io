---
title: "A Data-driven Deep Learning Approach for Bitcoin Price Forecasting"
collection: publications
category: conferences
permalink: /publication/2023
excerpt: "This paper is about Prediction of Bitcoin price with Deep Learning <br/> <img src='/parth-modi.github.io/images/bitcoin.gif'>"
date: 2023-06-11
venue: '2023 24th International Conference on Digital Signal Processing (DSP), Rhodes, Greece'
paperurl: 'https://www.researchgate.net/publication/372147431_A_Data-driven_Deep_Learning_Approach_for_Bitcoin_Price_Forecasting'
citation: 'P. D. Modi, K. Arshi, P. J. Kunz and A. M. Zoubir, "A Data-driven Deep Learning Approach for Bitcoin Price Forecasting," 2023 24th International Conference on Digital Signal Processing (DSP), Rhodes (Rodos), Greece, 2023, pp. 1-4, doi: 10.1109/DSP58604.2023.10167930.'
---
![Bitcoin Deployment]({{site.baseurl}}/images/bitcoindeployment.png)
<p align="center"><em>Figure 1: Real Time Price Prediction</em></p>
Bitcoin as a cryptocurrency has been one of the most important digital coins and the first decentralized digital currency. We propose a shallow Bidirectional-LSTM (Bi-LSTM) model, fed with feature engineered data using our proposed method to forecast bitcoin closing prices in a daily time frame. We compare the performance with that of other forecasting methods, and show that with the help of the proposed feature engineering method, a shallow deep neural network out-performs other popular price forecasting models.

| Model              | MAE Train | RMSE Train | MAE Test | RMSE Test | MAPE Test |
|--------------------|-----------|------------|----------|-----------|-----------|
| SVR                | 239.83    | 380.78     | 738.69   | 898.22    | 0.04      |
| XG Boost           | 106.39    | 170.26     | 1502.74  | 1829.44   | 0.03      |
| Linear Regression  | 250.08    | 383.18     | 562.19   | 691.23    | 0.03      |
| LSTM               | 167.27    | 288.14     | 479.77   | 650.81    | 0.04      |
| Bi-LSTM            | 160.76    | 279.93     | 414.51   | 561.76    | 0.03      |

For more details, refer to the [GitHub repository](https://github.com/Parth527/Bitcoin-Forecasting).
