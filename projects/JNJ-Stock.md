---
layout: post
title: 'JNJ Stock Price What-if Analysis and Forecasting'
---
**Project Overview**

*The project objective is to forecast the stock price of JNJ at the end of 2019 based on contextual factors
*Conducted research in politics, economic, sociocultural and medical fields to collect relevant time serious data
*Performed data cleaning and data integrated with ETL tools; Prepared data for modeling via Alteryx and Python
*Built forecast model with 0.84 𝑅" by using time series model ARIMA and Linear Regression model
*Built multi-parameter and interactive Tableau dashboard for JNJ stock monthly price through 5 years till 2020
<br><br>
**Overview about JNJ (Johnson & Johnson)**

JNJ is one of the world’s largest healthcare company. Its products fall into three segments: 
*Pharmaceutical, with 39% of total sales 
*Medical device and diagnostic, with 36% 
*Consumer product, with 25%
<br><br>
![](https://raw.githubusercontent.com/haoyingy/Home/gh-pages/assets/img/projects/proj-2/JNJ.jpg)
**Explore Factors**

There are external factors and internal factors which will influence JNJ stock price. As internal factors are highly related to JNJ stock price, it’s hard to make time series prediction on it, so I focused on external factors to make prediction.
External factors for JNJ, there are two types:
<br>
***Competitive:***

As JNJ is world’s top Pharmaceutical company, and barriers to ‘Pharmaceutical, Medical device and diagnostic’ entry is very high, so new entrants or existing competitors have very small impact on JNJ, this type can be ignored. 
<br><br>
***Contextual:***

Politics, Economic (GDP, income, expenditure), sociocultural (aging population, surging rate of various health problem), technological, medical industries, health care cost, etc. So contextual factors will be my main focus. 
<br>
**Model building process**

I mainly used log_linear regression to build the model with ARIMA and ETS to predict time series data. I built the prediction model and what-if model through Alteryx. More details can be find [here]
<br><br>
***Alteryx Work Flow***
![](https://raw.githubusercontent.com/haoyingy/Home/gh-pages/assets/img/projects/proj-2/what-if.png)
![](https://raw.githubusercontent.com/haoyingy/Home/gh-pages/assets/img/projects/proj-2/alteryx-workflow.png)

Dependent variable:
* JNJ stock price (monthly) 
Independent variables:
* GDP per capita (quarterly)
* Income per capita (monthly)
* Health care construction cost (monthly) 
* Consumer Price Index for medical care (monthly) 
* Medical care commodities price index (monthly) 
(data source: [fred.stlouisfed](https://fred.stlouisfed.org/))

**Result and Insight**

After modeling, I planted what-if model result into Tableau, then we can build a What-if Dashboard, on which we can change our predictors and forecast date to simulate the price change. <br>
***what-if dashboard***

![](https://raw.githubusercontent.com/haoyingy/Home/gh-pages/assets/img/projects/proj-2/what-if-vis.png)
<br>
The following shows the change trend line of predictors. The data is from forecast modeling using ARIMA and ETS time series models. <br>
***Predictors Forecast***

![](https://raw.githubusercontent.com/haoyingy/Home/gh-pages/assets/img/projects/proj-2/predictor-forecast.png)
<br>
The following shows the final model forecast result. Through the model, the expected price for JNJ at the end of 2019 would be $152.00. which means 17% increase from last year. <br>

![](https://raw.githubusercontent.com/haoyingy/Home/gh-pages/assets/img/projects/proj-2/prediction.jpg)
<br><br>
For more details of this project, please find [here](https://github.com/haoyingyang)


