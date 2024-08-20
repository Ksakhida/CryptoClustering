# CryptoClustering

## Overview
This project leverages unsupervised learning techniques to analyze and cluster cryptocurrencies based on their price change percentages over 24-hour and 7-day periods. The primary goal is to determine if these price changes affect the grouping of cryptocurrencies.

## Project Structure
- **Crypto_Clustering.ipynb**: The main notebook containing the code for data loading, preprocessing, clustering analysis using K-means, and visualization of results.
- **crypto_market_data.csv**: The dataset used for analysis, containing cryptocurrency price changes.
- **README.md**: This file, providing an overview of the project and a summary of the analysis.

## Methodology
1. **Data Preprocessing**: The cryptocurrency data is normalized using StandardScaler to ensure all features contribute equally to the clustering process.
2. **K-Means Clustering**: The elbow method is applied to determine the optimal number of clusters, which is then used to group the cryptocurrencies.
3. **Principal Component Analysis (PCA)**: PCA is used to reduce the dataset's dimensionality, making it easier to visualize and potentially enhancing clustering performance.
4. **Visualization**: Scatter plots are generated to visualize the clusters formed both with and without PCA, offering insights into the impact of dimensionality reduction.

## Results
- **Optimal Clusters**: The elbow method identified 4 as the optimal number of clusters, both in the original data and after applying PCA.
- **PCA Impact**: The use of PCA reduced the feature space to 3 principal components, explaining 89.50% of the variance in the data. This reduction led to more distinct and easily identifiable clusters in the visualizations.

## Conclusion
The analysis revealed that while the elbow curves for both K-means clustering and PCA are remarkably similar, using PCA to reduce the number of features before clustering leads to clearer and more distinct clusters. By simplifying the dataset through PCA, the clustering process becomes more effective, allowing for better separation of groups, which may be less apparent when using all features in the original K-means clustering.

This demonstrates the importance of feature reduction in enhancing the clarity and effectiveness of clustering analysis. The insights gained from this analysis can be valuable for traders and investors in the crypto market, as it helps in identifying distinct groups of cryptocurrencies based on their price change behavior.
