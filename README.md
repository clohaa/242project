# Forecast COVID-19 vaccine demand around the world by predicting 7-day new cases trend

Problem Statement

Aim to predict COVID-19 new cases across the globe and identify high risk countries which has high demand for vaccine, based on factors which may strongly correlate with vaccination rates, demographic information, and economic status.

In a perfect scenario, the algorithm should be able to accurately determine countries with high risk and assist international bodies such as the W.H.O in allocating relief funds to nations in need of urgent care. This will help in optimizing funds and at the same time ensure maximum impact of the relief-focused initiatives.

Data

Main data set is from kaggle that describes COVID-19 vaccination,mortality rates and other variables by country from Dec 27, 2020 to Sept 25, 2021. https://www.kaggle.com/sinakaraji/covid-vaccination-vs-death

Also added additional information about each country described in the World Bank Open Data and IMF Data page to include GDP, demographics, and other descriptive statistics not included in the original dataset.
https://data.worldbank.org/
https://www.imf.org/en/Data 
https://www.kaggle.com/koryto/countryinfo

Model training strategy: Cluster-then-Predict

Step 1: Use unsupervised machine learning (Hierachical clustering) to identify countries in high-risk cluster 
Step 2: Use a time-series model (Random Forest ir ARIMA) to forecast 7-day new cases trend for the high-risk cluster

Impact and overall goal of the project

For this project, the goal is to create a method for understanding factors that have a strong impact on the covid 19 mortality rate around the world. While vaccination rates are clearly one of the main ways to understand this, we are also interested in investigating the impact of a country’s wealth, demographics, life expectancy, and other factors that could also contribute to higher mortality rates per population. 

This tool would help healthcare officals to prioritize high-risk countries when allocating resources such as humanitarian support and COVID vaccine
