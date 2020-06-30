# Precdict eCommerce price
## Goal
The blooming of eCommerce platforms over the last 2 decades makes the market become very competitive. To dominate the market they must provide customer with goods at a lower price. This project uses the data from an e-commerce platform to predict the goods price based on given features in the data. 

## Data
The data contains contains 2452 observations with 7 columns (features) and a target variable, _Selling_price_. The data is originally from _Machinehack_ hackathon. 

## Method
The exploratory data analysis (EDA) showed a highly skewed distribution of the selling price. The selling price was then transformed into a logarithmic scale. I did feature engineering as following:
- using Date column to create: Day of Week, Month, Quarter, etc
- using groupby function and statical method, for example, Rating column, number of unique items at each brand, category
- encoding some features

I used XGBRegressor model to predict the target. XGBoost is a decision-tree-based ensemble Machine Learning algorithm. It uses a gradient boosting framework. 

## Requirement
The EDA and modeling were performed in Python 3 with Jupyter Notebook. The flowing is some necessary libraries, packages:
   - Pandas, numpy
   - Matplotlib, seaborn
   - Sklearn, xgboost.
   
## Results

## The reasons for the calls

![Image description](https://github.com/lamdoanduc/Machine-Learning-Projects/blob/master/Predict_eCommerce_Price/plots/results_1.png)

## Charts showing number of calls by Month, Day of Week highlighted by Reason column

![Image description](https://github.com/lamdoanduc/911-Calls/blob/master/Plots/calls_by_time.png)

## Linear Fit showing number of calls by month: groupby data by Month, then using count() funtion

![Image description](https://github.com/lamdoanduc/911-Calls/blob/master/Plots/Number_of_calls_by_Month.png)

## Number of calls by days for the entire period

![Image description](https://github.com/lamdoanduc/911-Calls/blob/master/Plots/Number_of_calls_by_time.png)

## The cluster shows high time of 911 calls

![Image description](https://github.com/lamdoanduc/911-Calls/blob/master/Plots/heatmap.png)


