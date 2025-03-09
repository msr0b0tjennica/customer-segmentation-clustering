# Customer Segmentation Using K-Means Clustering

## Overview
This project aims to segment customers into distinct groups based on their purchase records. We utilize K-Means clustering and apply Principal Component Analysis (PCA) for visualization.

## Dataset
The dataset used for this project is `Mall_Customers.csv`, which contains customer demographic information and spending patterns.

## Steps Involved
1. **Data Preprocessing:**
   - Load the dataset and check for missing values.
   - Drop the `CustomerID` column as it does not contribute to clustering.
   - Encode categorical variables (e.g., `Gender`).
   - Standardize the numerical features using `StandardScaler`.

2. **Finding the Optimal Number of Clusters:**
   - Use the **Elbow Method** to determine the optimal value of `k`.
   - Utilize the `KneeLocator` library to locate the elbow point.

3. **Applying K-Means Clustering:**
   - Train the K-Means algorithm with the optimal `k` value.
   - Assign cluster labels to the dataset.

4. **Visualizing the Clusters:**
   - Apply **PCA (Principal Component Analysis)** to reduce dimensionality to 2 components and plot the clusters.
   - Use **t-SNE (t-Distributed Stochastic Neighbor Embedding)** for an alternative visualization of clusters.

5. **Cluster Analysis:**
   - Analyze cluster characteristics by computing mean values for each group.

## Libraries Used
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `sklearn.cluster.KMeans`
- `sklearn.decomposition.PCA`
- `sklearn.manifold.TSNE`
- `sklearn.preprocessing.StandardScaler`
- `kneed.KneeLocator`

## Results
- The optimal number of clusters was determined using the Elbow Method.
- Customers were successfully segmented into clusters.
- PCA and t-SNE were used to visualize the clusters effectively.
- The segmented groups can be analyzed for targeted marketing strategies.

## How to Run
1. Install required dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn kneed
   ```
2. Load and preprocess the dataset.
3. Run the clustering algorithm and analyze results.
4. Visualize clusters using PCA and t-SNE.

## Future Enhancements
- Experiment with other clustering algorithms like **DBSCAN** or **Agglomerative Clustering**.
- Use **Silhouette Score** to further validate clustering results.
- Apply **customer behavioral analysis** based on spending patterns.

---
**Author:** Your Name

**License:** MIT License

