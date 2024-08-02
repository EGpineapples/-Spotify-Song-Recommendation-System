# Spotify Recommendation System

## Overview
This project implements a Spotify song recommendation system using an ensemble of four main content-based methods:
1. K-Means Clustering
2. Decision Trees
3. Cosine Similarity
4. Locality Sensitivity Hashing (LSH)

The system analyzes song features and lyrical content to provide personalized music recommendations.

## Dataset
- Main dataset: 170,653 songs with 19 features
- Lyrics dataset: 18,454 songs

## Methodology
1. Data Preprocessing:
   - Feature selection (14 quantitative features)
   - Standardization
   - Principal Component Analysis (PCA) for dimensionality reduction

2. K-Means Clustering:
   - Optimal cluster number determined using Davies-Bouldin Index
   - Used for initial song grouping

3. Decision Tree:
   - Custom implementation
   - Used for classification based on PCA features

4. Cosine Similarity:
   - Measures similarity between song vectors

5. Locality Sensitivity Hashing (LSH):
   - Analyzes lyrical content for similarity

6. Ensemble Method:
   - Combines recommendations from all four methods using majority voting

## Key Features
- Multi-modal analysis (audio features and lyrics)
- Ensemble approach for robust recommendations
- Custom implementation of machine learning algorithms
