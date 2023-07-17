# Beginners Trading Bot

### Motivation & Hypothesis
This backend project is intended to create a trading bot that implements different strategies taught by the author. While one learns different trading strategies, the knowledge can be passed on to the bot who can run them during market hours, whenever applicable. As you teach the bot more, its capabilities and efficiency increases with it. Emphasis on profitability and scalability is essential, as we intend to produce a reliable money making machine.
---
### Trading Strategies Used
#### Strategy 1: Overview
Our First strategy searches for the following 6 price patterns, which signals a trade entry:

- Bullish 'Quasi' Engulfing
- Bearish 'Quasi' Engulfing

- Bullish 'Neutral' Harami
- Bearish 'Neutral' Harami

- Bullish Double Candlestick LOW, with Higher HIGH and Higher CLOSE
- Bearish Double Candlestick LOW, with Higher HIGH and Higher CLOSE


![image_480](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/c1be7f4f-1203-4e6e-af85-37b19f149336)


We also implemented Initial Stop Losses (ISL)s to maximize profits and protect ourselves from unexpected changes in the market.
explain?

---
### Strategy 1: Test Findings 
We reviewed our coding logic by looking at the market data, and using machine learning models to evaluate and confirm our theories. We have found that our code is close to 100% accurate at predicting trade entries and exits, as confirmed by machine learning evaluation scores.


#### Support Vector Classifier
![svc_be](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/72f36014-5ad8-4f23-8c51-7f726a329044)
![svc_b_exit](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/219cff21-005d-4f1c-af57-894812e6c1b5)
![svc_se](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/8fe59839-2828-4667-965f-6180c576f4c3)
![svc_s_exit](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/559bcab6-7990-46b8-a1b9-f21e5ea364b6)



#### Decision Tree Cassifier
![dtc_buy_entry](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/bffac718-f2f6-4858-9754-be274e157861)
![dtc_buy_exit](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/ecd0227d-2744-4634-8140-04663571cc17)
![dtc_sell_entry](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/f6db8385-31ae-40d6-8f00-cad866631575)
![dtc_sell_exit](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/7ea56100-03a1-4859-8fd5-a46efb46443d)



#### Random Forrest Cassifier
![rfc_buy_entry](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/19a6b809-d91c-452a-945d-adefd634b6c5)
![rfc_buy_exit](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/70c0bb0b-8ccb-452f-9472-294cc4343b68)
![rfc_sell_entry](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/bb0c869a-313b-423d-9511-78fc9e5cecbf)
![rfc_sell_exit](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/ee72ab2f-0069-430b-9509-c93ab08039e9)


---
#### Potential Upgrades
- An objective Optimizer

![image_720](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/3e652b8e-62f5-4bb8-9775-11ed1b752f8b)


---
### Conclusion
---
#### Libraries Used

- Scikit Learn
  - Support Vector Machines
  - Random Forest Classifier
  - Decision Tree Classifier
- Plotly
- Matplotlib
- Numpy
- Pandas
- Alpaca Trade API
---

#### Contributors 
---
Pinda Johnson 

Dylan Brown

Branzil Engracia
