I would like to go through and practice on majority, if not all, of the models listed below. My ultimate goal is to gain comprehensive understanding and compile detailed notes for future use on each model. Lets go!

<img width="1000" alt="" src="https://github.com/user-attachments/assets/ffecf765-6f72-4035-8e1a-32a220772264">

----------

<img width="648" alt="featureScailing" src="https://github.com/user-attachments/assets/26810063-5498-4ebb-b307-92890e641ce5">
Credit: Super Data Science

Scaling/Normalizing the data often improves the performance of many machine learning models, especially those that are sensitive to the scale of the input features, such as:

- Linear Regression: Helps ensure that the model treats each feature equally.
- Logistic Regression: Assumes features are on a similar scale for better performance.
- Support Vector Machines (SVM): Sensitive to the scale of the data and performs better when the data is standardized.
- K-Nearest Neighbors (KNN): Distance-based algorithms like KNN are highly affected by the scale of the data.
- Principal Component Analysis (PCA): Assumes that the data is centered and scaled.

See Youtube video: https://www.youtube.com/watch?v=n9KeJLGwW0U&t=313s

- Use Normalization when you need to scale features to a fixed range, especially for algorithms that rely on distance metrics or when working with neural networks (KNN, K-Means, Neural Networks)
- Use Standardization when the data needs to be centered around zero with unit variance, especially for algorithms that assume normally distributed data or when features have different units (Linear Regression, Logistic Regression, SVM, PCA)
- Decision Trees, Random Forests, and Gradient Boosted Trees are generally not affected by feature scaling as they are based on hierarchical splitting and not distance measures.
 
Ultimately, the best approach is to experiment with both normalization and standardization, and validate the performance of your model using cross-validation.
