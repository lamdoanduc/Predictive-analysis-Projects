# A network intrusion detector
## Task:
* Build a predictive model capable of distinguishing between 'bad' connections, called intrusions or attacks, and 'good' normal connections.
* Differentiate between both the normal traffic and among distinct types of attack (predict the actual types (22 types) of attack).

## Data
* The dataset was acquired, by Lincoln Labs, for nine weeks of raw TCP dump data for a local-area network (LAN) simulating a typical U.S. Air Force LAN. [This Link](http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html) is for more information about the data.

## Workflow
* Start by visualizing the data to understand the data
* Use PCA and TNSE to do data for feature reduction and plot the data in 2D. This might help to show the data clusters and anomalies
* Perform feature engineering
* Use Random Forest, SVM, and ANN algorithms for binary classifiers to differentiate  'normal and 'attack' connections
* Predict the actual types of attack using multiple classifiers with Random Forest, SVM, and ANN algorithms

## Results
* The ML models showed very promising results on the test datasets. They can even detect some minor class attack. Overall, the Random forest model performed better compared to the two others in the dataset.

Click [the link](https://github.com/lamdoanduc/Predictive-analysis-Projects/blob/master/Network_intrusion_detector/code.ipynb) for the code.
