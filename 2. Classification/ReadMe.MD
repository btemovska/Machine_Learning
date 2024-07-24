<img width="745" alt="logistic" src="https://github.com/user-attachments/assets/14fdbb43-b6e3-4749-9d62-8948e03abdec">
Credit: Super Data Science

---------

<img width="700" alt="confusionMatrix2" src="https://github.com/user-attachments/assets/8def116a-b650-401e-9fef-5f419ff01fc4">
Credit: Skye Tran

- Accuracy - how often is the model correct? Caution - never use accuracy alone due to Accuracy Paradox (model achieves high accuracy but performs poorly in terms of other metrics that are more relevant to the problem at hand. This paradox typically arises in imbalanced datasets, where one class significantly outnumbers the other(s)). 
- Recall (aka sensitivity) - when it actually is positive case, how often is it correct? How many relevant cases are found? A lower or zero recall score will alert you that the model isn't catching relevant cases. 
- Precision - when prediction is positive, how often is it correct? Same in here, lower or zero score will alert you model isn't good. 
- F1 score - it is the harmonic mean of precision and recall. Essentially reports back how well are you doing in both Recall and Precision in one number.

---------

<img width="970" alt="KNN" src="https://github.com/user-attachments/assets/ecf1578b-00c3-4ddb-a5c6-453261b7b805">
Credit: Super Data Science

- Always choose off number of K to avoid tie between the classes
- How to choose how many Ks to choose? Is more better? Not quite - overall you want to minimize the Error 1 - Accuracy
        - option 1 - elbow method
        - option 2 - cross validate a grid search of multiple K values and choose K that reslts in lowest error or highest accuracy
Credit: Jose Portilla
