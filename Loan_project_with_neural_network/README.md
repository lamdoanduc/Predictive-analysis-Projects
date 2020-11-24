# Loan default detection using Neural network
## Our Goal
A model can predict wether or not a borrower will pay back his/her loan. The model is trained with a given historical data that has information on whether or not the borrowers defaulted. The model can be used in the future to assess if a new customer is likely to pay back the loan.

## Method
A deep neural network is used to address the problem. Since the data is imbalanced, it will be resampled (both under-sampled and over-sampled) to get better results of prediction. A random forest model is also performed for a comparison.

## Results
A deep neural network with a early stop method and Dropout shows a good performance.
Resampling the imbalanced data helps to improve the prediction on the minor class (class with a small number of observations).
A random forest model also performs well in this imbalanced dataset. However it underperforms the newral network trained by resampled data.

## Work flow
* First, exploratory data analysis
* Handle the missing data
* Feature engineering
* Data prepossessing
* Train and evaluate a deep neural network
* Tune the model with resampled data
* Train a random forest model for a comparison.


