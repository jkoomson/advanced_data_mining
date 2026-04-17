# 🔥 Wildfire Regime Analysis & Clustering
**Montesinho Natural Park (Portugal)**

## 📌 Project Overview

This project analyzes **wildfire behavior and fire regimes** in Montesinho Natural Park using **exploratory data analysis, unsupervised clustering, and spatial visualization** in **R**.

The objective is to identify **distinct fire regimes** based on weather conditions, seasonality, burned area, and spatial patterns, and to communicate these findings through **clear, reproducible, publication-quality visualizations**.

The final output includes:
- Fire regime clusters
- Seasonal patterns by cluster
- Spatial distribution across the park grid
- A compact, dashboard-style summary

---

## 📊 Data

- **517 wildfire events**
- Key variables:
  - Fire Weather Index components: `FFMC`, `DMC`, `DC`, `ISI`
  - Meteorological variables: temperature, relative humidity, wind
  - Burned area (log-transformed due to heavy right skew)
  - Temporal variables: month, day of week
  - Spatial grid coordinates (9×9 park grid)

Preprocessing steps include:
- Feature scaling and standardization
- Log transformation of burned area
- Ordered temporal factors for seasonal analysis

---

## 🧠 Methodology

### 1️⃣ Exploratory Data Analysis (EDA)
- Distributional analysis of fire weather variables
- Temporal trends by month and day of week
- Identification of extreme fire events

### 2️⃣ Unsupervised Clustering
- Feature normalization
- Model-based clustering using **`mclust`**
- Selection of the optimal number of clusters
- Interpretation of fire regimes

### 3️⃣ Cluster Profiling
- Standardized feature profiles by cluster
- Burned area comparison across fire regimes
- Cluster size and frequency analysis

### 4️⃣ Spatial Analysis
- Grid-based aggregation of fire events
- Dominant fire regime per grid cell
- Spatial intensity visualization using bubble maps

---

## 📈 Key Findings

- **Three distinct fire regimes** were identified:
  - **Cluster 1**: High-intensity fires under extreme weather conditions
  - **Cluster 2**: Moderate conditions with frequent small-to-medium fires
  - **Cluster 3**: Mild conditions with limited spread potential
- Fire occurrence is **strongly seasonal**, peaking in **August–September**
- Different fire regimes dominate **different spatial regions** of the park
- Large fires are rare but disproportionately influential for total burned area

---

## 🧰 Tech Stack

- **R**
- **tidyverse** (`dplyr`, `ggplot2`, `tidyr`)
- **mclust** – model-based clustering
- **caret** – machine learning workflows
- **patchwork** – dashboard-style visualization
- **Quarto / R Markdown** – reproducible reporting

---

## ⚠️ Reproducibility Notes

- Namespace conflicts (e.g., `dplyr::count()` vs `mclust::count()`) are explicitly handled
- Code is written to be **Posit Connect–safe**
- Computationally intensive steps are structured for caching or precomputation

---

## 📂 Repository Structure
