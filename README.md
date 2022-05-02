# Credit Risk Analysis
## Overview
The purpose of this analysis was to create a supervised machine learning model that could accurately predict credit risk. In order to complete this task, I used 6 different methods, which are:

1. Naive Random Oversampling
2. SMOTE Oversampling
3. Cluster Centroid Undersampling
4. SMOTEENN Sampling
5. Balanced Random Forest Classifying
6. Easy Ensemble Classifying

Through each of these methods, I split my data into training and testing datasets, and compiled accuracy scores, confusion matries, and classification reports as my results.

## Results
### Naive Random Oversampling
Accuracy Score: 67.4%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 72%
Recall Low Risk: 63%

Oversampling Analysis

![image](https://user-images.githubusercontent.com/95595378/166186682-b5a876e1-a7df-46fe-b3ca-704b9f1a223a.png)


### SMOTE Oversampling
Accuracy Score: 66.2%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 66%
Recall Low Risk: 66%

![image](https://user-images.githubusercontent.com/95595378/166187412-0ca14c8a-9c8a-4365-a092-7754838c6a44.png)


### Cluster Centroid Undersampling
Accuracy Score: 53.3%
Precision High Risk: 0%
Precision Low Risk: 100%
Recall High Risk: 61%
Recall Low Risk: 42%

![image](https://user-images.githubusercontent.com/95595378/166186874-64bb4d60-dd85-42dc-8cb5-4b2037dd43f7.png)

### SMOTEENN Sampling
Accuracy Score: 68.1%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 76%
Recall Low Risk: 60%

![image](https://user-images.githubusercontent.com/95595378/166186985-f1bf3e70-2ea7-43b9-8f02-a8039079f11a.png)

### Balanced Random Forest Classifying
Accuracy Score: 64.8%
Precision High Risk: 56%
Precision Low Risk: 100%
Recall High Risk: 30%
Recall Low Risk: 100%

![image](https://user-images.githubusercontent.com/95595378/166187195-cb11817f-9836-4d76-a25e-b419a1b4cd5a.png)

### Easy Ensemble Classifying
Accuracy Score: 92.3%
Precision High Risk: 6%
Precision Low Risk: 100%
Recall High Risk: 91%
Recall Low Risk: 94%

![image](https://user-images.githubusercontent.com/95595378/166187305-bfba826a-3ceb-4354-bcde-dedb26979170.png)

## Summary
This analysis is trying to find the best model that can detect if a loan is high risk or not. Becasue of that, we need to find a model that lets the least amount of high risk loans pass through undetected. That correlating statistic for this is the recall rate for high risk. Looking through the different models, the ones that scored the highest were:

1.Easy Ensemble Classifying (91%)

2.SMOTEENN Sampling (76%)

3.Naive Random Oversampling (72%)

While this is the most important statistic that is pulled from this analysis, another important statistic is recall rate for low risk as it shows how many low risk loans are flagged as high risk. Looking through the different models, the ones that scored the highest were:

1.Balanced Random Forest Classifying (100%)

2.Easy Ensemble Classifying (94%)

After taking these two statistics over the others, we can look at the accurary score to get a picture of how well the model performs in general. The models with the highest accuracy scores were:

1.Easy Ensemble Classify (92.3%)

2.SMOTEENN Sampling (68.1%)

3.Balanced Random Forest Classifying (64.8%)

After factoring in these three main statistics, the model that I would recommend to use for predicting high risk loans is the Easy Ensemble Classifying model.
