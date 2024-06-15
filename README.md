# Clustering Analysis for Vectorized Data

## Overview

This repository explores different clustering techniques applied to vectorized data using various vectorizers and clustering algorithms. The goal is to find natural groupings or clusters within the data based on different text representations.

## Table of Contents

- [Overview](#overview)
- [Table of Contents](#table-of-contents)
- [Clustering Results](#clustering-results)
  - [Kmeans Clustering](#kmeans-clustering)
  - [Agglomerative Clustering](#agglomerative-clustering)
  - [DBSCAN Clustering](#dbscan-clustering)

## Clustering Results

### Kmeans Clustering

| Vectorizer | Model              | Clusters |
|------------|--------------------|----------|
| BOW        | Kmeans Clustering  | 4        |
| TFIDF      | Kmeans Clustering  | 2        |
| AVG-W2V    | Kmeans Clustering  | 2        |
| TFIDF-W2V  | Kmeans Clustering  | 2        |

### Agglomerative Clustering

| Vectorizer | Model                      | Optimal_Clusters |
|------------|----------------------------|------------------|
| AVG-W2V    | Agglomerative Clustering   | 2                |
| AVG-W2V    | Agglomerative Clustering   | 5                |
| TFIDF-W2V  | Agglomerative Clustering   | 2                |
| TFIDF-W2V  | Agglomerative Clustering   | 5                |

### DBSCAN Clustering

| Vectorizer | Model                  | Min-pts | Eps   |
|------------|------------------------|---------|-------|
| AVG-W2V    | DBSCAN Clustering      | 50      | 2.594 |
| TFIDF-W2V  | DBSCAN Clustering      | 50      | 2.428 |

## Conclusion

This project demonstrates the application of various clustering algorithms on text data represented by different vectorization techniques. Each combination of vectorizer and clustering algorithm resulted in different optimal parameters or cluster counts, indicating the versatility and adaptability of clustering methods in identifying structure within text data.
