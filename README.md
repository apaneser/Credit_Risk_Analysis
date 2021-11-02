# Credit Risk Analysis
 
## Overview  
### Purpose  
The purpose of this project is to compare different machine learning models to see which ones are effecient in finding whether a person has low or high credit card risk. The dataset is unbalanced.

## Results  
Oversampling  
![Oversampling](Screenshots/Oversampling.PNG)  

SMOTE Oversampling  
![SMOTE](Screenshots/SMOTE_Oversampling.PNG)  

Undersampling  
![Undersampling](Screenshots/Undersampling.PNG)  

SMOTEENN (Oversampling + Undersampling)  
![SMOTEENN](Screenshots/SMOTEENN.PNG)  

Balanced Random Forest Classifier  
![Balanced Random Forest Classifier](Screenshots/Balanced_Random_Forest_Classifier.PNG)  

Easy Ensemble AdaBoost Classifier  
![Easy Ensemble AdaBoost Classifier](Screenshots/Easy_Ensemble_AdaBoost_Classifier.PNG)  

## Summary   
All the methods have low precision scores while the Easy Ensemblw Adaboost Classifier had the best Recall score for diagnosing high risk by a large margin, and also has the second highest precision score, despite still being a very low score of 0.08. Because of the high recall score, most of the people that actually have high credit risk will be diagnosed correctly with it. the downside is that the low precision score means that a large amount of people will be misdiagnosed to having high credit risk, so there will be many false positives. due to the importance of correctly diagnosing whether people have high credit rist, having a high recall value is more important than having a high precision score, so I would recommend using the Easy Ensemble Ada Classifier model as it can find the most people that have high credit risk.
