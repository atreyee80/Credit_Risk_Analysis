# Credit_Risk_Analysis
Create a machine learning model and analysis using different sampling techniques and the imbalanced-learn and scikit-learn libraries on the credit risk dataset from LendingClub by:  

1.Oversampling the data using the RandomOverSampler and SMOTE algorithms.<br> 
2.Undersampling the data using the ClusterCentroids algorithm.<br> 
3.Oversampling and undersampling the data using the SMOTEEN algorithm.<br> 
4.Comparing the two models that reduce bias to predice risk: BalancedRandomForestClassifier and EasyEnsembleClassifier.<br> 
5.Evaluate the performance of the models and their efficiency in predicting risk <br> 

#Resources
Data Sources provided to analyze and minipulate included:

.LoanStats_2019Q1.csv
.Software utilized for this study included:

.Python 3.7.6
.Conda 4.9.2
.Jupyter Notebook 6.1.4
.Personal GitHub account




## Comparison of Results- High Risk Of Default
|Model|Balanced Accuracy|High Risk Precision|High Risk Recall|SPE|F1|GEO|IBA|SUP|
|---|---|---|---|---|---|---|---|---|
|Formula|(TP+NP)/(TP+FP+TN+FN)|TP/(TP+FP)|TP/(TP+FN)
|---|---|---|---|
|RandomOverSampler|0.58|0.01|0.47|0.69|0.02|0.57|0.32|104|
|SMOTE|0.62|0.01|0.51|0.73|0.02|0.61|0.37|104|
|ClusterCentroids|0.54|0.01|0.58|0.50|0.01|0.54|0.29|104|
|SMOTEENN|0.63|0.01|0.66|0.60|0.02|0.63|0.40|104
|BalancedRandomForestClassifier|0.66|0.88|0.34|1.00|0.49|0.58|0.31|104|
|EasyEnsembleClassifier|0.91|0.09|0.89|0.94|0.16|0.92|0.84|104|



## Comparison of Results- Low Risk Of Default
|Model|Balanced Accuracy|High Risk Precision|High Risk Recall|SPE|F1|GEO|IBA|SUP|
|---|---|---|---|---|---|---|---|---|
|Formula|(TP+NP)/(TP+FP+TN+FN)|TP/(TP+FP)|TP/(TP+FN)
|---|---|---|---|
|RandomOverSampler|0.58|1.00|0.69|0.47|0.82|0.57|0.33|17101|
|SMOTE|0.62|1.00|0.73|0.51|0.85|0.61|0.38|17101|
|ClusterCentroids|0.54|0.99|0.50|0.58|0.67|0.54|0.29|17101|
|SMOTEENN|0.63|1.00|0.60|0.66|0.75|0.63|0.40|17101
|BalancedRandomForestClassifier|0.66|1.00|1.00|0.34|1.00|0.58|0.36|17101|
|EasyEnsembleClassifier|0.91|1.00|0.94|0.89|0.97|0.92|0.85|17101|




