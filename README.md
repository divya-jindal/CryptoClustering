# CryptoClustering Project

## Overview

This script performs clustering analysis on cryptocurrency market data using K-means clustering and Principal Component Analysis (PCA). The primary objectives are to determine the optimal number of clusters (k) and to visualize the clustering results with and without PCA optimization.

## Dependencies
* pandas
* hvplot
* scikit-learn

## Script Overview
### 1. Import Libraries
- pandas for data manipulation.
- hvplot.pandas for data visualization.
- KMeans from sklearn.cluster for clustering.
- PCA from sklearn.decomposition for dimensionality reduction.
- StandardScaler from sklearn.preprocessing for data normalization.
### 2. Load and Explore Data
- Data is loaded from a CSV file into a Pandas DataFrame.
- Displays sample data and generates summary statistics.
- Creates a line plot to visualize the data.
### 3. Data Preparation
- Normalizes the data using StandardScaler.
- Converts the scaled data back into a DataFrame with the original indices.
### 4. Finding Optimal k for Original Data
- Computes inertia values for k ranging from 1 to 10.
- Plots the Elbow curve to determine the optimal number of clusters.
### 5. Clustering with K-means (Original Data)
- Performs K-means clustering using the optimal k.
- Adds cluster labels to the DataFrame and visualizes clusters in a scatter plot.
### 6. PCA Optimization
- Reduces dimensionality using PCA with 3 components.
- Computes and displays the explained variance for each principal component.
- Creates a DataFrame with PCA-transformed data.
### 7. Finding Optimal k for PCA Data
- Repeats the process of finding optimal k using PCA-transformed data.
- Plots the Elbow curve for the PCA data.
### 8. Clustering with K-means (PCA Data)
- Performs K-means clustering on PCA-transformed data.
- Adds cluster labels to the DataFrame and visualizes clusters in a scatter plot.
### 9. Visualization and Comparison
- Compares the Elbow curves and clustering results

## Results Analysis
1. Optimal k Value: The optimal number of clusters (k) is found to be 4 for both the original and PCA-transformed data.
2. Impact of PCA: Using PCA helps in reducing the dimensionality, which can make clustering more interpretable and effective by removing noise.

## Usage
1. Update the path to the CSV file in the script.
2. Run the script to perform clustering analysis and generate visualizations.
3. Analyze the results and compare the impact of dimensionality reduction using PCA.

