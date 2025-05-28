# Pima Indians Diabetes Classification Improvement

## Overview
This repository contains a Python project that enhances the classification of the Pima Indians Diabetes dataset using a hybrid approach of unsupervised clustering and supervised classification. The goal was to improve upon the results presented in a reference research article.

## Project Goal
The project optimizes the classification of diabetic vs. non-diabetic cases by combining dimensionality reduction (PCA), clustering (K-Means, K-Means with PCA, MiniBatchKMeans, Spectral Clustering, BIRCH), and supervised learning with K-Nearest Neighbors (KNN). It achieves a test error rate of 24.03%, surpassing the original article's best performance of 26.85%.

## Improved Article
This work builds upon the methodology and results from the article:
- **Title**: Improving Clustering Method Performance Using K-Means, Mini Batch K-Means, BIRCH and Spectral
- **DOI**: https://doi.org/10.1109/ISRITI54043.2021.9702823
- **Reference Error Rates**: 26.85% to 28.52% (Table II)

Our implementation improves these error rates by optimizing clustering parameters (35-48 clusters) and enhancing KNN with `weights='distance'` and GridSearchCV.

## Installation
1. Clone the repository: `git clone https://github.com/yourusername/pima-diabetes.git`
2. Install dependencies
3. Run the script: `jupyter notebook classification.ipynb`

## Requirements
- Python 3.x
- Libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`

## Results
- Test Error Rate: 24.03% (K-Means, K-Means with PCA)
- 10-Fold CV Error Rate: 23.78% (Spectral Clustering)
