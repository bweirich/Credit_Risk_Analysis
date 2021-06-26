# Credit_Risk_Analysis

## Purpose
The purpose of this analysis is to create the best model to predict whether a loan is high risk or low risk based on different features associated with the applicant.  Since the dataset is unbalance with far more low risk loan risk we will use several techniques to handle the imbalance.  These techniques included over sampaling, undersampling, combination of oversampaling and undersampaling and then ensemble models to remove bias.

The performance of each model will be evaluated using the balanced accuracy score and the imbalanced classification report showing the precision and recall.

## Results

### Naive Random Oversampling (RandomOverSampler)
- Balanced Accuracy Score
 
![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/balance_over_sample.PNG)
- Imbalanced Classification Report

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/prec_recall_over_sample.PNG)

### SMOTE Oversampling
- Balanced Accuracy Score

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/balance_smote.PNG)
- Imbalanced Classification Report

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/prec_recall_smote.PNG)

### Undersampling (Cluster Centroids)
- Balanced Accuracy Score

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/balance_confusion.PNG)
- Imbalanced Classification Report

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/prec_recall_cluster.PNG)

### Combination Sampling (SMOTEENN)
- Balanced Accuracy Score

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/balance_smoteenn.PNG)
- Imbalanced Classification Report

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/prec_recall_smoteenn.PNG)

### Balanced Random Forest
- Balanced Accuracy Score

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/balance_balanced.PNG)
- Imbalanced Classification Report

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/prec_recall_balanced.PNG)

### Easy Ensemble Ada Boost
- Balanced Accuracy Score

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/balance_easy.PNG)
- Imbalanced Classification Report

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/prec_recall_easy.PNG)

## Summary
