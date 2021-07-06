# Credit_Risk_Analysis
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


