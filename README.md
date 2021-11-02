# Credit Risk Analysis
 
## Overview  
### Purpose  
The purpose of this project is to compare different machine learning models to see which ones are effecient in finding whether a person has low or high credit card risk. The dataset is unbalanced.

## Results  
Oversampling  
* Balanced accuracy score: 0.649  
![Oversampling](Screenshots/Oversampling.PNG)  

SMOTE Oversampling  
* Balanced accuracy score: 0.658  
![SMOTE](Screenshots/SMOTE_Oversampling.PNG)  

Undersampling  
* Balanced accuracy score: 0.545  
![Undersampling](Screenshots/Undersampling.PNG)  

SMOTEENN (Oversampling + Undersampling) 
* Balanced accuracy score: 0.648  
![SMOTEENN](Screenshots/SMOTEENN.PNG)  

Balanced Random Forest Classifier  
* Balanced accuracy score: 0.734  
![Balanced Random Forest Classifier](Screenshots/Balanced_Random_Forest_Classifier.PNG)  

Easy Ensemble AdaBoost Classifier  
* Balanced accuracy score: 0.915  
![Easy Ensemble AdaBoost Classifier](Screenshots/Easy_Ensemble_AdaBoost_Classifier.PNG)  

* All of the methods have hgih precision of either 1.0 or 0.99 for diagnosing people with low risk
* For Recall rates of people diagnosed with low rates, The Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier have the highest Recall rates above .90, followed by SMOTE with .68, SMOTEENN and Oversampling with .57, and the rest below .50
* Every method has very low precision for diagnosing people with high risk with the highest being Balanced Random Forest Classifier with 0.08 and Easy Ensemble Adaboost Classifier with 0.05
* For Reecall Rates of people diagnosed with high credit risk, Easy Ensemble AdaBoost Classifier has the highest rate by a large margin with a score of 0.93, followed by Oversampling with 0.73, SMOTEENN with 0.72, and the rest under 0.70

## Summary   
All the methods have low precision scores for diagnosing high risk by a large margin while the Easy Ensemblw Adaboost Classifier had the best Recall score, and also has the second highest precision score, despite still being a very low score of 0.08. Because of the high recall score, most of the people that actually have high credit risk will be diagnosed correctly with it. the downside is that the low precision score means that a large amount of people will be misdiagnosed to having high credit risk, so there will be many false positives. due to the importance of correctly diagnosing whether people have high credit rist, having a high recall value is more important than having a high precision score, so I would recommend using the Easy Ensemble Ada Classifier model as it can find the most people that have high credit risk.
