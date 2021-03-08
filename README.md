# Project: Advanced Time Series Forecasting of Cowboy Cigarettes Sales using ARIMA and SARIMA Models

![Time_series](https://user-images.githubusercontent.com/67468718/110270113-fd289e00-7f79-11eb-80aa-13e656231036.JPG)

## 1. Introduction

The US federal government - the Health and Environment department are investigating whether sales for the oldest and most powerful producers of cigarettes in the country are increasing or declining. 

**Cowboy Cigarettes (TM, *est.* 1890)** is the US's longest-running cigarette manufacturer. Like many cigarette companies, however, they haven't always been that public about their sales and marketing data. The available post-war historical data runs for only 11 years after they resumed production in 1949; stopping in 1960 before resuming again in 1970. 

So, in order to help them in the investigating, I will be using the 1949-1960 data to predict whether the manufacturer's cigarette sales actually increased, decreased, or stayed the same. I will be using the latest machine learning modelling techniques more specifically ARIMA and SARIMA models to make a probable reconstruction of the sales record of the manufacturer - predicting the future, from the perspective of the past - to contribute to a full report on US public health in relation to major cigarette companies. 

The results of our analysis will be used as part of a major report relating public health and local economics, and will be combined with other studies executed by your colleagues to provide important government advice.  

## 2. Time Series Defintion

Time series data is just any data displaying how a single variable changes over time. It comes as a collection of metrics typically taken at regular intervals. Common examples of time series data include weekly sales data and daily stock prices. You can also easily acquire time series data from [Google Trends](https://trends.google.com/trends/?geo=US), which shows you how popular certain search terms are, measured in number of Google searches. 

## 3. Visualizing predictor variable <code>**y**</code> using **Tableau**:


![cig_sales](https://user-images.githubusercontent.com/67468718/110266605-0104f200-7f73-11eb-9503-4f649935cdef.JPG)

## 4 The Box-Jenkins method

Building time series models can represent a lot of work for the modeler and so we want to maximize our ability to carry out these projects fast, efficiently and rigorously. This is where the Box-Jenkins method comes in. The Box-Jenkins method is a kind of checklist for you to go from raw data to a model ready for production. The three main steps that stand between you and a production-ready model are identification, estimation and model diagnostics:

**4.1 Identification:**
  * Is a Time Series stationary?
  * What differencing will make it stationary?
  * What transforms will make it stationary?
  * What values of <code>**p**</code> and <code>**q**</code> are most promising?
  
 
**4.2 Estimation:**
 * Estimate the <code>**AR**</code> and <code>**MA**</code> coefficients of the data by fitting the Model using <code>**.fit() method**</code>.
 * At this stage we might fit many models and use the AIC and BIC to narrow down to more promising candidates.
 
**4.3 Model Diagnostics:** 
 * Evaluate the quality of the fitting Model by using test statistics <code>**.summary() method**</code> and diagnostic plots <code>**.plot_diagnostics() method**</code> to make sure the residuals are well behaved!
 
![box_Jenkins](https://user-images.githubusercontent.com/67468718/110121273-0a277080-7d73-11eb-8315-f8b8eca62ad5.JPG)
