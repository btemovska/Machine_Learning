<img width="529" alt="equations" src="https://github.com/user-attachments/assets/b90d136d-6056-4845-903a-6900d695b7b5">
Credit: SuperDataScience

<img width="354" alt="graph" src="https://github.com/user-attachments/assets/83e14cb9-3098-4dcc-81ba-80c9406935e0">
Credit: Tavish



----------------------------------------------------------------------------------------
Asked ChatGPT why should we use sklearn.preprocessing import StandardScaler?

The StandardScaler from sklearn.preprocessing is used in machine learning and data preprocessing. The process ensures that your data is centered around 0 with a standard deviation of 1, which often improves the performance of many machine learning models, especially those that are sensitive to the scale of the input features, such as:
      - Linear Regression: Helps ensure that the model treats each feature equally.
      - Logistic Regression: Assumes features are on a similar scale for better performance.
      - Support Vector Machines (SVM): Sensitive to the scale of the data and performs better when the data is standardized.
      - K-Nearest Neighbors (KNN): Distance-based algorithms like KNN are highly affected by the scale of the data.
      - Principal Component Analysis (PCA): Assumes that the data is centered and scaled.

The formula used is:
    z-score is z = (x-μ)/σ   (where x is the original feature, 𝜇 μ is the mean of the feature, and 𝜎 σ is the standard deviation)

When do we know to use Scaler: 
- Especially around the models listed above, ex. KNN deals with distance (cm vs m)
- Decision Trees, Random Forests, and Gradient Boosted Trees are generally not affected by feature scaling as they are based on hierarchical splitting and not distance measures.

See Youtube video: https://www.youtube.com/watch?v=n9KeJLGwW0U&t=313s
