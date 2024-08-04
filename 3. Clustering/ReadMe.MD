Unsupervised ML - does not have y-label. There is only X-features in the dataset to cluster them. 

----------------------
"Clustering uses unlabeled data and looks for similarities between groups (clusters) in order to attemt to segment the data into separate clusters" - Credit:  Jose Portilla

----------------------
<img width="686" alt="clustering" src="https://github.com/user-attachments/assets/0c6ca979-fefa-4b50-bafd-8fcec2d8407d"> Credit: Super Data Science

----------------------
<img width="621" alt="k-means" src="https://github.com/user-attachments/assets/5ba1de4d-154c-4adb-9005-d53c7eb5bc8e">Credit: Super Data Science

1. Initialization: Choose the number of clusters, 𝑘. 
2. Initialize the centroids (means) of the clusters. This can be done randomly or by using some heuristic (e.g., k-means++).
3. Assignment Step: Assign each data point to the nearest centroid. This is done by calculating the Euclidean distance between each data point and each centroid, and assigning the point to the cluster with the closest centroid.
4. Update Step: Recalculate the centroids of the clusters. This is done by taking the mean of all the data points assigned to each cluster. The new centroid is the arithmetic mean of the points in the cluster.
5. Iteration: Repeat the Assignment and Update steps until the centroids no longer change significantly or a maximum number of iterations is reached. The algorithm has converged when the assignments no longer change or the change in the centroids is below a specified threshold.

----------------------
How to Evaluate the model?

# The Silhouette Score is a measure of how well each data point is clustered, ranging from -1 to 1: 
# Generally:
# 0.5 - 1.0: Good to excellent clustering, indicating that clusters are well-separated and coherent.
# 0.25 - 0.5: Moderate clustering, suggesting some overlap or poor separation between clusters.
# Below 0.25: Poor clustering, indicating a high degree of overlap or inappropriate clustering.

# positive number (closer to 1) means very well clustered
# negative number (closer to -1) means incorrectly clustered
