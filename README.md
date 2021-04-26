# Credit Risk Analysis

## Overview of the analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we will employ different techniques to train and evaluate models with unbalanced classes. In this project we will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

## Methodology
In the first few models, I oversampled the data using randomoversampler and smote algorithms and undersample the data with the clustercentroid algorithm and in the remaining models,I used a combination approach to over and undersample the data using smoteenn. Finally, I compared two machine learning models that minimize bias, balancedrandomforestclassifier and easyensembleclassifier. 

## Results
1. Naive Random oversampling
Our balanced accuracy test it 66%, the precision for the high risk has a very low positivity at 1% and the recall is 66%.
![Capture](https://user-images.githubusercontent.com/76858662/116026280-5fb82500-a620-11eb-81ee-afea095feac7.PNG)

2. Smote oversampling
Our balanced accuracy score is 62%, the precision for the high risk loans has a low positvity again at 1% and recall is 66% overall
![Capture1](https://user-images.githubusercontent.com/76858662/116026461-d0f7d800-a620-11eb-8508-1e02722941c8.PNG)

3. Undersampling
Our balanced accuracy score is 51% overall, the precision is at 99% and the recall is 45%
![Capture2](https://user-images.githubusercontent.com/76858662/116026806-61361d00-a621-11eb-8f4e-34009f58ca15.PNG)

4. Combination(over and undersampling)
Our balanced accuracy score is 63.7%, the precision is 99% and the recall is 57% overall
![Capture](https://user-images.githubusercontent.com/76858662/116027037-de619200-a621-11eb-80b1-ee83f04ab808.PNG)

5. Balanced Random Forest Classifier 
Our balanced accuracy score is 74.9% the precision is 99% and the recall is 88%
![Capture](https://user-images.githubusercontent.com/76858662/116027182-33050d00-a622-11eb-8e35-5c105dc56565.PNG)

6. Easy Ensemble AdaBoost Classifier
Our balanced accuracy score is 91.7% the precision is 99% and the recall is 94%
![Capture](https://user-images.githubusercontent.com/76858662/116027282-752e4e80-a622-11eb-969f-e4709204679a.PNG)

## Summary
In the initial four models, we did undersampled, oversampled and combination of both, in order to determine which model is best at predicting what loans are at the highest risk. In the next two models, we resampled the data using ensemble classifiers to predict which loans are at high or low risk. In the initial four models, our accuracy score is not as high as the ensemble classifiers. 
Typically in our models, we want a adequate balance of recall and precision. In my opinion, I would recommend the ensemble classifiers over the rest of the models as it seems to high accuracy score and nice balance of precision and recall scores.






