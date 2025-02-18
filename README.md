# K-means Clustering on FIFA 22 Player Dataset

In this project, I performed K-means clustering on the FIFA 22 player dataset to identify patterns among players. The clustering process grouped players based on their overall rating, potential, wage, value, and age. The results helped me understand different clusters of players, such as star players, younger players, and older players.

### Loaded the Dataset
I loaded the FIFA 22 player dataset using the pandas library. The `low_memory=False` parameter ensured that the dataset was read efficiently, even if there were mixed data types.

### Selected Features for Clustering
I focused on five key features for clustering: overall rating, potential, wage (in euros), value (in euros), and age. These features were essential in determining the players' performance and market value.

### Cleaned the Dataset
I removed any rows that had missing values in the selected features to ensure the data was clean and ready for clustering.

### Scaled the Data
I scaled the data using Min-Max scaling to ensure all feature values were within the range of 1 to 10. This step was crucial to prevent any single feature from dominating the clustering process.

### Initialized Random Centroids
I randomly initialized centroids for the clusters. Centroids are the central points of each cluster and were updated during the clustering process.

### Labeled Data Points Based on Centroid Distance
I assigned each data point (player) to the nearest centroid based on the Euclidean distance. This step labeled each player according to the closest centroid.

### Updated Centroids
I updated the centroids by calculating the geometric mean of the data points in each cluster. This ensured that the centroids represented the center of the players' features in each cluster.

### Repeated the Clustering Process
I repeated the steps of labeling data points and updating centroids until the centroids no longer changed or a maximum number of iterations was reached. This iterative process ensured that the clusters were well-defined and stable.

### Visualized Clusters
I used Principal Component Analysis (PCA) to reduce the dimensionality of the data from five dimensions to two. This allowed me to visualize the clusters on a 2D plot. I plotted the data points and centroids for each iteration to observe how the clusters evolved.

### Analyzed Results
I analyzed the final centroids and the players in each cluster to understand the patterns. For example, I identified which clusters represented star players, younger players, or older players.
