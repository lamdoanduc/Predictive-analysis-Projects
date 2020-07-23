# Exploring an Ecommerce Dataset exported from Google Analytics

## 1. Goals
### 1.1. Exploratory data analysis
* Number of views and number of unique users
* Top ten products with the most views
* Top top 10 selling products
* Number of different eCommerceAction_type
* Calculate revenue by month
* How many % of the total visitors made a purchase?
* How many visitors bought on subsequent visits to the website?

### 1.2. Predictive analysis

There are customers who add products to carts but they removed the products from the carts or logged out without further processing. The customers don't complete the purchases. I try to create a LM model to predict whether the customers will complete the purchases after adding products to carts.

## 2. Data

The public dataset in BigQuery is exported from Google Analytics 360 data from the Google Merchandise Store. For more information, click [Here](https://console.cloud.google.com/marketplace/product/obfuscated-ga360-data/obfuscated-ga360-data?filter=solution-type:dataset&q=ecommerce&id=45f150ac-81d3-4796-9abf-d7a4f98eb4c6&project=qwiklabs-gcp-04-42fd9c021ec6&folder=&organizationId=). The data includes the following information:
* Traffic source data: information about where website visitors originate, including data about organic traffic, paid search traffic, and display traffic
* Content data: information about the behavior of users on the site, such as URLs of pages that visitors look at, how they interact with content, etc.
* Transactional data: information about the transactions on the Google Merchandise Store website.

## 3. Method
I use Google Bigquery and Chart inside Notebook in DataLab to perform the exploratory data analysis and ML classification model. Logistic regression which is supported inside Bigquery is selected for the classification model. 

## Results

The results from the exploratory data analysis are shown in the tables and plots in the code attached below. The value of _roc-auc_ in the classification model is about 0.7. 

## Requirement

One needs a GCP account to access Google Bigquery and DataLab. This public dataset is hosted in Google BigQuery and is included in BigQuery's 1TB/mo of free tier processing. 

## Files
The report and code can be found [Here](https://github.com/lamdoanduc/Predictive-analysis-Projects/blob/master/Exploring_Google_Analytics_Dataset/report_code.ipynb)
