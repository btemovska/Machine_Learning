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
### How to Evaluate the model?

OPTION 1
The Elbow Method helps determine the optimal number of clusters by plotting the sum of squared distances (or inertia) from each point to its assigned cluster center as a function of the number of clusters. Pick the cluster where the rate of decrease in inertia sharply shifts.

OPTION 2 
The Silhouette Score measures how similar each data point is to its own cluster compared to other clusters, ranging from -1 to 1: 
Generally:
- 0.5 - 1.0: Good to excellent clustering, indicating that clusters are well-separated and coherent.
- 0.25 - 0.5: Moderate clustering, suggesting some overlap or poor separation between clusters.
- Below 0.25: Poor clustering, indicating a high degree of overlap or inappropriate clustering.

- positive number (closer to 1) means very well clustered
- negative number (closer to -1) means incorrectly clustered


OPTION 3 
The Davies-Bouldin Index (DBI) is a metric used to evaluate the quality of clustering. It measures the average similarity ratio of each cluster with the cluster most similar to it. Lower values indicate better clustering performance, as they suggest that clusters are well-separated and compact.
- Less than 1: Typically considered excellent clustering.
- between 1 and less than 2: Good clustering, but improvements may be possible.
- between 2 and less than 5: Fair clustering with noticeable issues.
- greater 5: Poor clustering; significant issues with cluster separation or compactness.

------------
<img width="800" alt="hierarchialClustering" src="https://github.com/user-attachments/assets/fa3404ce-e605-4895-a59a-4055f2307c1a">
Credit: DataCamp

------------
#### DBSCAN - Densitiy-based spatial clustering of applications with noise is a powerful technique which can be used for clustering and outlier detection. Credit: Jose Portilla

