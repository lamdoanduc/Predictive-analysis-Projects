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

## Cross validation score
The final model got the cross-validation score is about 0.7. 
The distribution of the difference between the predicted price and the real values is shown in the left-hand side plot. The right-hand side scatter-plot shows the prediction vs the reality.

![Image description](https://github.com/lamdoanduc/Machine-Learning-Projects/blob/master/Predict_eCommerce_Price/plots/results_1.png)

## Feature importances 
The summary of feature importances is shown in the below plot. 

<img align="center" width="500" height="300" src="https://github.com/lamdoanduc/Machine-Learning-Projects/blob/master/Predict_eCommerce_Price/plots/results_2.png">




