<img width="827" alt="ML" src="https://github.com/user-attachments/assets/f824a831-4ecd-40f5-b8f9-7076ef149982">

----------


Scaling/Normalizing the data often improves the performance of many machine learning models, especially those that are sensitive to the scale of the input features, such as:

- Linear Regression: Helps ensure that the model treats each feature equally.
- Logistic Regression: Assumes features are on a similar scale for better performance.
- Support Vector Machines (SVM): Sensitive to the scale of the data and performs better when the data is standardized.
- K-Nearest Neighbors (KNN): Distance-based algorithms like KNN are highly affected by the scale of the data.
- Principal Component Analysis (PCA): Assumes that the data is centered and scaled.

See Youtube video: https://www.youtube.com/watch?v=n9KeJLGwW0U&t=313s

- Use Normalization when you need to scale features to a fixed range, especially for algorithms that rely on distance metrics or when working with neural networks (KNN, K-Means, Neural Networks). "Another common method to scale data is normalization, which rescales the data to a zero to one range. Unlike the standardized data, all the normalized data is on a positive scale." (Ankur A. Patel, 2019)
- Use Standardization when the data needs to be centered around zero with unit variance, especially for algorithms that assume normally distributed data or when features have different units (Linear Regression, Logistic Regression, SVM, PCA). "Standardization has mean of of zero and standard deviation of one. Some machine learning solutions are very sensiitve to the scale of the data, so having all the data on the same relative scale - via standardization - is a good machine learning practice." (Ankur A. Patel, 2019)
- Decision Trees, Random Forests, and Gradient Boosted Trees are generally not affected by feature scaling as they are based on hierarchical splitting and not distance measures.
 
Ultimately, the best approach is to experiment with both normalization and standardization, and validate the performance of your model using cross-validation.




----------
Ordinal Encoding:
	- Satisfaction levels (satisfied: 3, neutral: 2, dissatisfied: 1)
	- Shipment Priority (high: 1, medium: 2, low: 3)
	
Label Encoding:
	- Colors (red: 1, blue: 2, green: 3).
	- Payment Method (CreditCard: 1, Paypal: 2)	
 
One-Hot Encoding:
	- Creates a new binary variable (0 or 1) for each category.

 TransactionEncoder:
 	- turn each product into True/False value (used for apriory algoritham)



----------
  Sources:
  (Ankur A. Patel, 2019) Hands-On Unsupervised Learning Using Python. O'Reilly Media.
