# Credit_Risk_Analysis - LendingClub

## Overview

Employ different techniques to train and evaluate models with unbalanced classes. Using the credit card credit dataset from LendingClub,
a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and under sample 
the data using the Cluster Centroids algorithm. Then, you’ll use a combinatorial approach of over- and under sampling using the SMOTEENN 
algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, 
to predict credit risk.

## Results

The following results are presented in a descending level for performance, based on their Balance Accuracy Scores along with the Imbalance 
Classification Report for each model. Since we are primarily interested to detect high credit risk individuals, the “f1” (F-score column) 
“avg/Total” as well as its result for the high-risk individuals.


- **Cluster Centroids Undersampling** is giving the lower score with an accuracy score of .5365

![image](https://user-images.githubusercontent.com/105381777/191658079-982aafdf-4f67-46d4-af01-53d1dfb30897.png)

Achieving an average of only .57 and an F-score for high-risk prediction of .01

![image](https://user-images.githubusercontent.com/105381777/191658151-1eb3d574-fa7e-4c47-ba0f-da87800c6013.png)


-	**Combination Sampling** with an accuracy score of .6483

![image](https://user-images.githubusercontent.com/105381777/191658210-cfa9917f-44d3-4002-8a0b-c417691a5772.png)

Achieving an average of only .73 and an F-score for high-risk prediction of .02

![image](https://user-images.githubusercontent.com/105381777/191658256-66ecdc76-f504-487f-ad08-f395de129216.png)


- SMOTE Oversampling with an accuracy score of .6587

![image](https://user-images.githubusercontent.com/105381777/191658348-eee3b97f-60a5-4b2d-a2d5-9b62f411ffc9.png)

Achieving an average of only .80 and an F-score for high-risk prediction of .02

![image](https://user-images.githubusercontent.com/105381777/191658413-d4bfd86e-d472-4997-bdeb-0dc635cdede9.png)


- **Naive Random Oversampling** with a better accuracy score of .6660  still close to the Combination Sampling and SMOTE Oversampling 

![image](https://user-images.githubusercontent.com/105381777/191658489-da48aec2-284c-4ce1-91a4-0adc0fa934dd.png)

This ROS model achieved an average of .77 and a F-score high-risk prediction of only .002

![image](https://user-images.githubusercontent.com/105381777/191658540-bf9bed1b-b27f-4373-9fa1-8111e867b419.png)


- **Balanced Random Forest Classifier** providing one of best results with an accuracy score of .7615

![image](https://user-images.githubusercontent.com/105381777/191658611-fb1686d2-c149-4fff-a793-077089fd6506.png)

Achieved an average of .92 and a F-score high-risk prediction of only .006

![image](https://user-images.githubusercontent.com/105381777/191658655-545a4812-142e-40f0-9bb3-246d193aab45.png)


- **Easy Ensemble AdaBoost Classifier** being the best-performing model with an accuracy score of .9319

![image](https://user-images.githubusercontent.com/105381777/191658895-2acef666-d6b8-47f8-a4c1-ad9ab192f83a.png)

The EEC model achieved an average F-score of 0.97. However, while this is the best performing, it's F-score for high-risk 
prediction was still low, at only 0.16

![image](https://user-images.githubusercontent.com/105381777/191659085-2174cdf5-01f0-4a36-ab5a-a084a1ec25b5.png)


## Summary

In summary, credit-risk is a very difficult to predict. Even with and Easy Ensemble AdaBoost Classifier model with the better 
accuracy average F-score above 90% but a F-score for high-risk predictions of .16.




