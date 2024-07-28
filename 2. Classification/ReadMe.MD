<img width="648" alt="featureScailing" src="https://github.com/user-attachments/assets/26810063-5498-4ebb-b307-92890e641ce5">    Credit: Super Data Science

The StandardScaler from sklearn.preprocessing is used in machine learning and data preprocessing. The process ensures that your data is centered around 0 with a standard deviation of 1, which often improves the performance of many machine learning models, especially those that are sensitive to the scale of the input features, such as:

- Linear Regression: Helps ensure that the model treats each feature equally.
- Logistic Regression: Assumes features are on a similar scale for better performance.
- Support Vector Machines (SVM): Sensitive to the scale of the data and performs better when the data is standardized.
- K-Nearest Neighbors (KNN): Distance-based algorithms like KNN are highly affected by the scale of the data.
- Principal Component Analysis (PCA): Assumes that the data is centered and scaled.

The formula used is: z-score is z = (x-μ)/σ (where x is the original feature, 𝜇 μ is the mean of the feature, and 𝜎 σ is the standard deviation)

When do we know to use Scaler:

- Especially around the models listed above, ex. KNN deals with distance (cm vs m)
- Decision Trees, Random Forests, and Gradient Boosted Trees are generally not affected by feature scaling as they are based on hierarchical splitting and not distance measures.

See Youtube video: https://www.youtube.com/watch?v=n9KeJLGwW0U&t=313s

- Use Normalization when you need to scale features to a fixed range, especially for algorithms that rely on distance metrics or when working with neural networks (KNN, K-Means, Neural Networks)
- Use Standardization when the data needs to be centered around zero with unit variance, especially for algorithms that assume normally distributed data or when features have different units (Linear Regression, Logistic Regression, SVM, PCA)
 
Ultimately, the best approach is to experiment with both normalization and standardization, and validate the performance of your model using cross-validation.

---------

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

<img width="970" alt="KNN" src="https://github.com/user-attachments/assets/ecf1578b-00c3-4ddb-a5c6-453261b7b805"> Credit: Super Data Science

KNN is almong the simplest algorithms, as it predicts on the basis of its closest neighbors in the training set. 

Always choose odd number of K to avoid tie between the classes
How to choose how many Ks to choose, is more better? Not quite - overall you want to minimize the Error 1 - Accuracy
- option 1 - elbow method
- option 2 - cross validate a grid search of multiple K values and choose K that reslts in lowest error or highest accuracy

Credit: Jose Portilla

Always do Feature Scaling on KNN as it is impacted by distance. And it is never a bad thing to use Feature Scaling.


---------

<img width="800" alt="SVM" src="https://github.com/user-attachments/assets/8640ce11-e1df-4591-a622-3f123cd07756"> Credit: Super Data Science

SVM is one of the complex algorithms .
Support Vector Classifier (with Soft Margins) - it is the kernels to project data to higher dimension to separate the data. 


---------

<img width="800" alt="DecisionTree" src="https://github.com/user-attachments/assets/88139e3e-02cd-4ad8-84a1-21f91e7f01b2">Credit: Super Data Science









