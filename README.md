## creditCardFraud


It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

### Dataset

https://www.kaggle.com/mlg-ulb/creditcardfraud

Content
The datasets contains transactions made by credit cards in September 2013 by european cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.
### Data Visualization
The graph below shows the visualization of the correlation matrix.
It seems that there are no strong co-relationship between each attributes,
![r2](https://user-images.githubusercontent.com/54567577/107547900-dc3f7980-6b82-11eb-80e6-de1aa5bb1b4a.png)

### Data Preprocessing

##### Reove Outliers
As the graph shown below, there are outlier in the dataset.
Outliers are remove to perform better ML accuracy.
![r1](https://user-images.githubusercontent.com/54567577/107547568-7226d480-6b82-11eb-9664-05dde3b06f02.png)

##### 

### Result

#### Logistic Regression
![result](https://user-images.githubusercontent.com/54567577/107547376-38ee6480-6b82-11eb-902f-7388d6406559.png)

Given the class imbalance ratio, the competition recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC)

AUC score is:  0.9536957405093118
Precision, Recall, Accuracy and AUC scores are excellent
