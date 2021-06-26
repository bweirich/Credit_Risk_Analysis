# Credit_Risk_Analysis

## Purpose
The purpose of this analysis is to create the best model to predict whether a loan is high risk or low risk based on different features associated with the applicant.  Since the dataset is unbalance with far more low risk loan risk we will use several techniques to handle the imbalance.  These techniques included oversampling, undersampling, combination of oversampling and undersampling and then ensemble models to remove bias.

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

### Easy Ensemble AdaBoost
- Balanced Accuracy Score

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/balance_easy.PNG)
- Imbalanced Classification Report

![alt_text](https://raw.githubusercontent.com/bweirich/Credit_Risk_Analysis/main/images/prec_recall_easy.PNG)

## Summary
As shown in the above scores the oversampling, undersampling and combination models performed roughly the same. The precision scores was the exact same for all of these models and the recall and balanced accuracy scores for comparative.  

The ensemble models performed higher on the balanced accuracy score with the Easy Ensemble AdaBoost model performing the best with a 93.18% accuracy.  The recall score of the Easy Ensemble AdaBoost model also shows the highest score at 92% for high risk loans.  The precision score for all models was very low when determining high risk loans with the Easy Ensemble AdaBoost model performing the best with a 9% score.  

For this analysis recall is the more important score as we want to flag all of the high risk loans even if this includes some false positives of low risk loans being flagged as high risk.  Even with this being said I would not recommend using any of these models.  There should be a better balance between the precision and recall scores and with the precision score being so low this model will not be able to successfully perform predictions and further models should be explored.
