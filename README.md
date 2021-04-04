
<h1 align="center">Credit Risk Analysis</h1>

## Overview
The purpose of this analysis is to visualize machine learning technique and logistic regression to build a model to detect high risk credit profiles.

## Results
The dataset shows an imbalanced split between high risk cases (small portion) and low risk cases (large portion). As such, the analysis has tried 6 different models and below are the results by model.

### 1. Random Oversampling
In random oversampling, instances of the minority class are randomly selected and added to the training set until the majority and minority classes are balanced. 

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/1_oversampling.PNG)

This model is not ideal as indicated by its low precision score for high risk class and the overall F1 score. The confusion matrix also showed that the model mis-classified 7,412 high risk cases to be low risk cases. 

### 2. SMOTE
In the synthetic minority oversampling technique (SMOTE), the size of the minority is increased by interpolating new instances. That is, for an instance from the minority class, a number of its closest neighbors is chosen. Based on the values of these neighbors, new values are created.

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/2_Smote.PNG)

Although a slight improvement from random oversampling, this model is not ideal as indicated by its low precision score for high risk class and a low overall F1 score. The confusion matrix allo showed that the model mis-classified 5,291 high risk cases to be low risk cases. 

### 3. Undersampling Cluster Centroids
Cluster centroid undersampling identifies clusters of the majority class, then generates synthetic data points, called centroids, that are representative of the clusters. The majority class is then undersampled down to the size of the minority class.

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/3_Undersampling.PNG)

Undersampling is highly ineffective given the limited number of cases. This model is not ideal as indicated by its low precision score for high risk class and a low overall F1 score. The confusion matrix also showed that the model mis-classified 10,324 high risk cases to be low risk cases, the worst among all models. 

### 4. SMOTEENN
SMOTEENN combines the SMOTE and Edited Nearest Neighbors (ENN) algorithms. SMOTEENN is a two-step process:
1. Oversample the minority class with SMOTE.
2. Clean the resulting data with an undersampling strategy. If the two nearest neighbors of a data point belong to two different classes, that data point is dropped.

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/4_overandunder.PNG)

This model is comparable to the first model but with a lower accuracy score. It again suffers from a low precision score for high risk class and a low overall F1 score. The confusion matrix also showed that the model mis-classified 10,324 high risk cases to be low risk cases, the worst among all models. 
 
### 5. Random Forest
A random forest algorithm will sample the data and build several smaller, simpler decision trees. Then, many slightly better than average small decision trees are combined to create a strong learner, which has much better decision making power.

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/5_randomForest.PNG)

This model is a significant improvement from all the above models. Even though, its recall score is still a low 0.36, which resulted in a modest F1 score of 0.52. But it is somewhat acceptable. 

### 6. Easy Ensemble
Easy ensemble is not a method that was covered in the module. The classifier is an ensemble of AdaBoost learners trained on different balanced boostrap samples. The balancing is achieved by random under-sampling.

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/6_Easy_Ensemble.PNG)

This model is also a significant improvement from the first four models. Tts recall score is still a low 0.36, which resulted in a modest F1 score of 0.52. But it has a better accuracy score than Random Forest model.



## Summary:

In Summary, the analysis shows that under sampling generally doesn't work well. Random Forest and Easy Ensemble models are noticeably better than all other models. If I have to choose one, I'd choose the Easy Ensemble, given its overall better performance. To further enhance it, one may consider dropping the features that showed low importance.

