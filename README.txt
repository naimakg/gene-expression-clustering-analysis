========================================
Gene Expression Clustering Analysis
========================================

Overview
--------

This notebook performs a gene expression clustering analysis to identify gene expression patterns before and after the diauxic shift.  
Several clustering algorithms, including K-means, Gaussian Mixture Models (GMM), Ward, and Birch, are applied to analyze the data.  
The notebook explores different clustering configurations, visualizes the results, and compares the performance of each algorithm.

The primary goal of this analysis is to identify clusters of genes that exhibit similar expression patterns over time.  
This will help in understanding the changes in gene expression related to the diauxic shift.

Key Steps
---------

- Preprocessing: Handle missing values and normalize the data.
- Visualization: Apply visualization techniques to explore the data distribution and relationships.
- Clustering: Apply K-means, GMM, Ward, and Birch clustering algorithms.
- Dimensionality Reduction: Use PCA to represent and visualize the data in a lower-dimensional space.
- Evaluation: Compare the clustering results and choose the optimal number of clusters.
- Filtering: Identify the most affected genes by the diauxic shift and re-cluster the data.
- Drawing conclusions: Summarize the findings and the performance of the algorithms.

Requirements
------------

- Python 3.11.4
- Jupyter Notebook (or JupyterLab)
- Anaconda (recommended for managing environments)

Required Libraries
------------------

Make sure the following libraries are installed:

- `numpy`==1.24.3
- `pandas`==1.5.3
- `matplotlib`==3.7.1
- `seaborn`==0.12.2
- `scikit-learn`==1.3.0

Data
----

The dataset includes gene expression data across different time points, including:

- Gene names
- Gene expression levels at several time points

Usage Instructions
------------------

1. Clone or download this repository.
2. Open the notebook (`gene_expression_clustering_analysis.ipynb`) in a Jupyter environment.
3. Run the cells sequentially.

Summary of Results
------------------

- Before filtering: 3 clusters were optimal, grouping genes based on increasing, decreasing, or stable expression.
- After filtering: 2 clusters were found, separating genes that increase or decrease expression over time.
- Best Algorithm: Birch worked best for unfiltered data, while K-means and GMM were more effective after filtering.

License
-------

This project is copyrighted by Naim Abdul Khalek Gharzeddine and is provided with all rights reserved. You may not use, modify, or distribute this code without explicit permission.
