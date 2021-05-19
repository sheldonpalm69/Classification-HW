# Classification of Risk Using Machine Learning
![Risk](https://raw.githubusercontent.com/sheldonpalm69/Classification-HW/main/Images/Credit-Risk-4.jpg)

#### UM FinTech BootCamp 2021

#### May 15th, 2021

---

#### Prepared by:

- Sheldon Palm

---

## Classification using Resampling
Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, a client has asked for assistance to predict credit risk with machine learning techniques.

This assignment I will build and evaluate several machine learning models to predict credit risk using data you'd typically see from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans) To evaluate the risk involved I will employ different techniques for training and evaluating models with imbalanced classes. Using the imbalanced-learn and Scikit-learn libraries the following techiques will be used:
- Simple Logistic Regression (SLR)
- Oversampling, Naive Random Over Sampling (NRO)
- SMOTE Oversampling 
- Undersampling/Cluster Centroids
- SMOTEENN Combination (Over and Under) Sampling 

All results will be reveiw to and evalauated by the resulting metrics as per their accuracy score. Classification report and confusion matrix are printed to compare models, to detirmine which set of data is the best fit for generating loan risk factors.

To generate loan risk I:
- Read the provided CSV data
-  Process the Data
- Scale the training and testing data using the StandardScaler from sklearn.
![CSV_DATA](https://raw.githubusercontent.com/sheldonpalm69/Classification-HW/main/Images/Load_CSV.png)


#### Simple Logistic Regression (SLR)
![Simple Logistic Regression](https://raw.githubusercontent.com/sheldonpalm69/Classification-HW/main/Images/SLR.png)


#### Oversampling, Naive Random Over Sampling (NRO)
![NRO](https://raw.githubusercontent.com/sheldonpalm69/Classification-HW/main/Images/NRO.png)


#### SMOTE Oversampling.
![SMOTE](https://raw.githubusercontent.com/sheldonpalm69/Classification-HW/main/Images/SMOTE.png)


#### Undersampling/Cluster Centroids
![CLCS](https://raw.githubusercontent.com/sheldonpalm69/Classification-HW/main/Images/CLCS.png)



#### SMOTEENN Combination (Over and Under) Sampling
![SMOTEENN](https://raw.githubusercontent.com/sheldonpalm69/Classification-HW/main/Images/SMOTEEN.png)

**The objective of this assignment is to apply these machine learning models, and be able to conclusively address the below questions:**

#### Questions and Answer
Of the 5 models, the Logistic Regression model using the SMOTEENN Combination Re-Sampler had the best balanced accuracy score at 99.4%.
Of the 5 models, the Naive Random Oversampling and the SMOTEEN both has a perfect score of 1.0.
Of the 5 models, both the Logistic Regression model using the SMOTEENN Combination Re-Sampler and the model using the Smote Oversampler had the best geometric mean scores at 79%.

## Classification using Ensemble Learners 
Using Ensemble Learners, I  will compare two ensemble algorithms to determine which algorithm results in the best performance. 
- Balanced Random Forest Classifier 
- Easy Ensemble Classifier

In order to reach valuable risk scores I will use the same CSV data to train the model.
- Calculate the balanced accuracy score from sklearn.metrics.
- Display the confusion matrix from sklearn.metrics.
- Generate a classication report using the imbalanced_classification_report from imbalanced-learn.
- Print the feature importance sorted in descending order



Of the 2 models, the Easy Ensemble classifier had the best balanced accuracy score at 92.5%.
Of the 2 models, the Easy Ensemble classifier had the best recall score at 91%.
Of the 2 models, the Easy Ensemble classifier had the best geometric mean score at 93%.
The top three features are total_rec_prncp (8.3%), total_pymnt_inv (6.9%) and last_pymnt_amnt (6.1%).


Data Set
[lending_data](https://github.com/sheldonpalm69/Classification-HW/blob/main/lending_data.csv)
[loan_stats](https://github.com/sheldonpalm69/Classification-HW/blob/main/LoanStats_2019Q1.csv)



###### References

- https://www.investopedia.com/

