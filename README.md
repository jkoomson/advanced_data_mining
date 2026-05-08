# Uncovering Hidden Fire Patterns: An Advanced Clustering Analysis of Wildfire Data

## Project Overview

Wildfires are complex environmental events influenced by the interaction of weather conditions, fuel dryness, wind behavior, and long-term drought accumulation. While traditional wildfire studies often focus on prediction or individual environmental variables, much of the hidden structure in wildfire behavior remains difficult to detect using conventional analysis alone.

This project applies advanced unsupervised machine learning techniques to uncover latent wildfire patterns using the UCI Forest Fires dataset, which contains 517 wildfire events recorded in Montesinho Natural Park, Portugal.

The primary objective of this study is to determine whether wildfire events naturally organize themselves into distinct behavioral regimes based on meteorological and fire-weather conditions — without providing the algorithms with predefined labels or categories.

To accomplish this, seven clustering algorithms were implemented and compared:

- K-Means
- Hierarchical Clustering
- DBSCAN
- Gaussian Mixture Models (GMM)
- Spectral Clustering
- Fuzzy C-Means
- CLARA

The analysis includes extensive preprocessing, feature engineering, standardization, dimensionality reduction, cluster validation, spatial visualization, and interpretability analysis.

---

## Key Features of the Project

### Advanced Unsupervised Learning Framework
This project demonstrates a comprehensive clustering workflow using seven fundamentally different machine learning algorithms spanning:
- centroid-based clustering,
- density-based clustering,
- probabilistic clustering,
- graph-based clustering,
- fuzzy clustering,
- and robust medoid-based clustering.

---

### Feature Engineering
Several derived variables were created to better capture wildfire behavior, including:
- logarithmic burned area transformation,
- drought load indices,
- and composite fire danger measures.

---

### Cluster Validation
Multiple validation techniques were used to determine the optimal number of clusters:
- Elbow Method
- Silhouette Analysis
- Gap Statistic

Internal validation metrics such as:
- Silhouette Score,
- Dunn Index,
- and Calinski–Harabasz Index

were also used to evaluate clustering quality across all methods.

---

### Spatial and Seasonal Analysis
The project includes:
- wildfire spatial mapping,
- seasonal trend analysis,
- cluster profile visualization,
- and interactive geographic exploration of wildfire regimes.

---

## Main Findings

Despite major differences in mathematical assumptions across all seven clustering algorithms, the methods consistently converged toward a stable three-cluster structure.

The discovered wildfire regimes can be interpreted as:

### 1. High-Intensity Drought-Driven Fires (“Summer Infernos”)
- Extreme drought accumulation
- High temperatures
- Low humidity
- Largest burned areas

### 2. Wind-Driven Rapid Spread Fires
- High spread potential
- Elevated wind influence
- Fast-moving fire conditions

### 3. Mild and Manageable Fires
- Lower drought stress
- Lower fire intensity
- Smaller burned areas
- More moderate environmental conditions

One of the strongest findings of the study is the dominant role of long-term drought accumulation, captured by the Drought Code (DC), in distinguishing severe wildfire conditions.

---

## Technologies Used

### Programming Language
- R

### Major Libraries
- tidyverse
- cluster
- factoextra
- dbscan
- mclust
- e1071
- kernlab
- dendextend
- corrplot
- leaflet
- patchwork
- GGally
- kableExtra

---

## Project Components

The project includes:
- data preprocessing,
- exploratory data analysis,
- feature engineering,
- clustering implementation,
- validation analysis,
- cluster interpretation,
- spatial visualization,
- interactive mapping,
- and comparative algorithm evaluation.

---

## Applications

This work has practical relevance for:
- wildfire risk assessment,
- climate analytics,
- environmental monitoring,
- disaster preparedness,
- resource allocation,
- and catastrophic risk modeling.

The project also demonstrates how unsupervised machine learning can uncover meaningful environmental structures hidden within high-dimensional data.

---

## Dataset Source

Cortez, P. and Morais, A. (2007).  
*A Data Mining Approach to Predict Forest Fires using Meteorological Data.*  
University of Minho, Portugal.

UCI Machine Learning Repository:
https://archive.ics.uci.edu/ml/datasets/forest+fires

---

## Author

John Koomson

Research Interests:
- Machine Learning
- Statistical Learning
- Environmental Risk Analytics
- Catastrophic Risk Modeling
- Unsupervised Learning
- Data Science
