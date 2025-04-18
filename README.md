# PREDICTIVE_ANALYSIS
Comparative Analysis of Clustering Algorithms
This repository contains a comprehensive analysis of different clustering algorithms using various pre-processing techniques and evaluation metrics.
Project Overview
The goal of this project is to compare the performance of different clustering algorithms on the Iris dataset from the UCI Machine Learning Repository. The analysis includes:

Applying multiple clustering algorithms (K-Means, Hierarchical, Mean Shift)
Testing various pre-processing techniques (No Processing, Normalization, PCA, etc.)
Evaluating performance with different numbers of clusters (c=3, c=4, c=5)
Measuring clustering quality using standard evaluation metrics

Dataset
The analysis uses the Iris dataset, which contains 150 samples with 4 features (sepal length, sepal width, petal length, petal width) across 3 species of Iris flowers.

Name: Iris Dataset
Source: UCI Machine Learning Repository
Link: https://archive.ics.uci.edu/ml/datasets/iris
Features: 4
Samples: 150
Classes: 3

Methodology
Clustering Algorithms

K-Means Clustering: A centroid-based algorithm that partitions the data into K clusters by minimizing the within-cluster sum of squares.
Hierarchical Clustering: An agglomerative clustering approach that builds nested clusters by merging or splitting them successively.
Mean Shift Clustering: A density-based clustering algorithm that identifies clusters by finding dense regions in the data.

Pre-processing Techniques

No Data Processing: Raw data without any pre-processing.
Normalization: Using StandardScaler to standardize features.
Transform: Using MinMaxScaler to scale features to a specific range.
PCA: Principal Component Analysis for dimensionality reduction.
T+N: A combination of normalization followed by transformation.
T+N+PCA: A combination of normalization, transformation, and PCA.

Evaluation Metrics

Silhouette Score: Measures how similar an object is to its own cluster compared to other clusters. Higher is better.
Calinski-Harabasz Index: The ratio of between-cluster dispersion to within-cluster dispersion. Higher is better.
Davies-Bouldin Index: The average similarity between each cluster and its most similar cluster. Lower is better.

Results
Performance Tables
The complete performance results are available in the clustering_results.csv file. Key findings include:

Best Silhouette Score: K-Means with PCA preprocessing and c=3 (Score: 1.0)
Best Calinski-Harabasz Index: K-Means with Normalization and c=5 (Score: 7999)
Best Davies-Bouldin Index: Hierarchical with PCA and c=3 (Score: 0.09)

Visualizations
The repository includes various visualizations to help understand the clustering results:

Feature Distribution Plots: Shows the distribution of each feature across the three Iris species.
Cluster Visualization Plots: Displays the clusters formed by different algorithms in 2D space (after PCA).
Performance Comparison Charts: Compares the different algorithms, pre-processing techniques, and cluster numbers.
Heatmaps: Visualizes the performance metrics for each configuration.

Key Findings

Optimal Cluster Number: The performance metrics consistently showed better results when the number of clusters matched the natural groupings in the data (c=3 for the Iris dataset).
Impact of Pre-processing: Dimensionality reduction using PCA
