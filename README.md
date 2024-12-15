I would like to go through and practice on majority, if not all, of the models listed below. My ultimate goal is to gain comprehensive understanding and compile detailed notes for future use on each model. Lets go!

<img width="827" alt="ML" src="https://github.com/user-attachments/assets/f824a831-4ecd-40f5-b8f9-7076ef149982">

----------


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




----------
Ordinal Encoding:
	- Satisfaction levels (satisfied: 3, neutral: 2, dissatisfied: 1)
	- Shipment Priority (high: 1, medium: 2, low: 3
	
	from sklearn.preprocessing import OrdinalEncoder
	order_priority_encoder = OrdinalEncoder(categories=[['High', 'Medium']])
	df['OrderPriority_Encoded'] = order_priority_encoder.fit_transform(df[['OrderPriority']]).astype(int)
	
Label Encoding:
	- Colors (red: 1, blue: 2, green: 3).
	- Payment Method (CreditCard: 1, Paypal: 2)
	
	from sklearn.preprocessing import LabelEncoder
	payment_encoder = LabelEncoder()
	df['PaymentMethod_Encoded'] = payment_encoder.fit_transform(df['PaymentMethod'])
	
One-Hot Encoding:
	- Creates a new binary variable (0 or 1) for each category.
