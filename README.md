# Beginners Trading Bot

### Motivation & Hypothesis
This backend project is focused on developing a trading bot that incorporates a variety of strategies. By transferring acquired knowledge and strategies to the bot, it becomes capable of executing trades during market hours. as we add to the strategy taught, the bot's capabilities and efficiency continue to improve. The primary objective is to create a reliable and profitable trading tool that can swiftly respond to market conditions and capitalize on lucrative trading opportunities.


Additionally, our beginner trading bot possesses the ability to analyze vast quantities of data and generate real-time trading signals. This feature enhances decision-making speed, enabling traders to make more prompt and informed choices.

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
- A Profit Optimizer Experiment

Displayed below is a **sample graphic** that can be utilized for upcoming experiments aimed at optimizing profits.

![image_720](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/3e652b8e-62f5-4bb8-9775-11ed1b752f8b)


As an example, we conducted a test on AAPL using an hourly time frame with a profit objective of 0.5. This test resulted in a profit of $4.09. However, when we shortened the time frame and adjusted the profit objective to 1.0 on a minute-by-minute basis, we observed a significant increase in profit, reaching $13.67. It is worth noting that when we further increased the profit objective to 2.0, the overall profit decreased. This led us to explore multiple variations to identify the optimal settings for maximizing profit potential. By continuously experimenting with different parameters, we strive to ensure that we generate the highest possible profit.

---
### Conclusion

- In conclusion, the trading bot has demonstrated success in backtesting, and therefore, we have decided to deploy it to a live trading account. To ensure its ongoing performance, the bot will be closely monitored on a regular basis.
- As part of future enhancements, we plan to launch the bot on the AWS platform, which will provide scalability and reliability.
- Additionally, we are exploring the incorporation of additional technical indicators such as Fibonacci retracements, Keltner channel bands, and moving averages to further enhance the bot's trading capabilities.
- During our analysis, we discovered that there is a point of diminishing returns, and we are dedicated to determining the optimal trading parameters to achieve the best possible results.
- Furthermore, we have concluded that this trading bot has the potential to be utilized in various markets, offering flexibility and adaptability.
- It's important to note that certain costs and expenses, including tax fees, and service provider fees, have not been fully accounted for in our evaluation. These factors should be considered when implementing the bot in live trading.
- Overall, we are excited about the potential of this trading bot and remain committed to continuous monitoring, optimization, and exploring further opportunities for improvement.


#### Charts:
![counter_sell_trend_1](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/7dcfbc98-29f2-4320-b8ba-a0aa5f90a3e9)
![counter_trend_buy](https://github.com/Pindainc/Beginners_Trading_Bot/assets/100908888/25c61142-8ec7-460e-9648-a6ac632af4f3)


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

#### Contributors: 
Pinda Johnson 

Dylan Brown

Branzil Engracia
