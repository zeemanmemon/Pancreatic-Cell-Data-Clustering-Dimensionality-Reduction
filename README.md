# Pancreatic Cell Data Clustering with Dimensionality Reduction

This repository explores the application of various dimensionality reduction techniques and clustering algorithms on the **Muraro dataset**, which contains single-cell RNA sequencing data from the human pancreas.

## Overview

High-dimensional biological data often suffer from challenges like the curse of dimensionality, making analysis and clustering inefficient. This repository implements techniques like **PCA**, **kPCA**, **Autoencoders**, **t-SNE**, and **UMAP** for dimensionality reduction and applies **k-means clustering** to identify distinct cell types in the dataset.

### Objectives:
- Address computational challenges in analyzing high-dimensional data.
- Apply dimensionality reduction techniques to preserve data structure.
- Evaluate clustering performance using **silhouette scores**.

## Dataset

The **Muraro dataset** was used in this research. It provides single-cell RNA sequencing data of the human pancreas. Preprocessing was applied to reformat the dataset for dimensionality reduction.

## Methodology

### Dimensionality Reduction Techniques:
1. **PCA**: Linear method preserving maximum variance.
2. **kPCA**: Non-linear extension of PCA using kernel functions.
3. **Autoencoders**: Neural network-based encoding and decoding.
4. **t-SNE**: Non-linear dimensionality reduction for visualization.
5. **UMAP**: Captures local and global structures efficiently.

### Clustering:
- **k-means clustering** was applied on the reduced data to group cells into distinct clusters.
- **Silhouette scores** were used to evaluate the quality of clusters.

## Results

- **UMAP** achieved the highest silhouette scores, indicating superior clustering performance.
- Non-linear techniques like kPCA and UMAP outperformed linear methods in preserving data structures.
- The optimal number of clusters was consistently identified as four for kPCA-transformed data.

## Future Work

- Hybrid approaches combining techniques like PCA and Autoencoders.
- Integration of advanced deep learning models like GANs.
- Scaling the methodology to larger, more diverse datasets.
