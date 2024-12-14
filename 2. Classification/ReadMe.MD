Logistics Regression


---------

<img width="700" alt="confusionMatrix2" src="https://github.com/user-attachments/assets/8def116a-b650-401e-9fef-5f419ff01fc4">
Credit: Skye Tran

- Accuracy - how often is the model correct? Caution - never use accuracy alone due to Accuracy Paradox (model achieves high accuracy but performs poorly in terms of other metrics that are more relevant to the problem at hand. This paradox typically arises in imbalanced datasets, where one class significantly outnumbers the other(s)). 
- Recall (aka sensitivity) - when it actually is positive case, how often is it correct? How many relevant cases are found? A lower or zero recall score will alert you that the model isn't catching relevant cases. 
- Precision - when prediction is positive, how often is it correct? Same in here, lower or zero score will alert you model isn't good. 
- F1 score - it is the harmonic mean of precision and recall. Essentially reports back how well are you doing in both Recall and Precision in one number.

---------

KNN



KNN is almong the simplest algorithms, as it predicts on the basis of its closest neighbors in the training set. 

Always choose odd number of K to avoid tie between the classes
How to choose how many Ks to choose, is more better? Not quite - overall you want to minimize the Error 1 - Accuracy
- option 1 - elbow method
- option 2 - cross validate a grid search of multiple K values and choose K that reslts in lowest error or highest accuracy

Credit: Jose Portilla

Always do Feature Scaling on KNN as it is impacted by distance. And it is never a bad thing to use Feature Scaling.


---------

SVM


SVM is one of the complex algorithms .
Support Vector Classifier (with Soft Margins) - it is the kernels to project data to higher dimension to separate the data. 


---------

Decision Tree for Classification

---------
Random Forest for Classification

Instead of running one Decision Tree, run multiple Trees model into one big model. Pick subset of Tree create Decision model, then pick another Tree and create Decision Model. This is known as Ensemble Learning (multiple Decision Tree models into one model). Once you get the predictions for each Tree, then you tally up and if most of the predictions says it belongs to class 0 then it is 0, if most predictions say it belongs to class 1 then it is 1. Can also know the predicted probability (ex. if Tree 1 says it is class 0, Tree 2 is class 0, and Tree 3 is class class 1, then it looks like it belongs to class 0 with 2/3rds probability). Where in Regression, if Tree 1 says it is 10 and Tree 2 says it is 13 and Tree 3 says it is 11, then sum these and divide by num of trees which is 11.3. 

- Number of Estimators - how many decision tree to use in total?
- Number of Features - how many features to include in each subset?
- Boostraping - random sampling with replacement
- Out of Bag Error - because of boot strap sampling, some of the rows did not make it that boot strap sampling, and for those we can calculate the error/score. It is optional way of measuring performance, an alternative to using standard train/test split (Credit: Jose Portilla)

---------
Boosting - another method of improving on the single Decision Tree. Boosting is known for Meta-learning (Meta-learning, often referred to as "learning to learn," is a subfield of machine learning where the aim is to improve the learning algorithms themselves by leveraging past experiences.)

<img width="515" alt="adaBoost" src="https://github.com/user-attachments/assets/ba242e36-857a-4152-9126-d11012599455">
Credit: Towards Data Science

Geadient Boosing - similar to AdaBoost, except it makes use of residual error based on previous model. Credit: Jose Portilla



