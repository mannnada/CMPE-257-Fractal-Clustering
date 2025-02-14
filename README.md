# CMPE-257-Fractal-Clustering
# Fractal Clustering Project

## Overview
This project applies **fractal clustering** to identify the **golden cluster** within a dataset. The approach involves recursive clustering, assessing clusters using predefined objective functions, and evaluating results using **Sum of Squared Errors (SSE)** and **Silhouette Score**.

## Objectives
- Implement **fractal clustering** on a dataset.
- Define **two objective functions** to determine when to stop re-clustering.
- Compute **SSE (Sum of Squared Errors)** and **Silhouette Score** to evaluate cluster quality.
- Analyze the results to determine the **golden cluster**.

## Data Narrative
### Key Questions
- **Business Task:** How can we effectively segment data using fractal clustering for optimal decision-making?
- **ML Task:** Clustering - identifying meaningful groups in data.
- **Data Representation:** Numerical tabular format with relevant features (e.g., financial, healthcare, customer segmentation).

## Datasets
### 1. Downloaded Dataset
- **Source:** Structured dataset from an external source (CSV format).

### 2. Scraped Dataset
- **Specification for web scraping:**
  - **Target:** `[Specify website/API]`
  - **Fields:** `[List the features to extract]`
  - **Tools:** `BeautifulSoup`, `Scrapy`, `Selenium` (if needed)

## Implementation Steps
1. Load and preprocess the dataset.
2. Apply **K-Means clustering** to segment the data.
3. Define and apply **fractal clustering**:
   - Recursively cluster data within larger groups.
   - Evaluate each cluster using objective functions.
   - Stop re-clustering when optimal clusters are found.
4. Compute evaluation metrics:
   - **SSE (Sum of Squared Errors)**: Measures intra-cluster variance.
   - **Silhouette Score**: Evaluates separation between clusters.
5. Identify and analyze the **golden cluster**.

## Objective Functions for Golden Cluster
### 1. Compactness Objective
- Measures cluster density.
- **Formula:** `Compactness = (Σ D_i) / N`, where `D_i` is the distance of points to the cluster center.

### 2. Separation Objective
- Measures how distinct a cluster is from others.
- **Formula:** `Separation = (Distance to nearest cluster) / (Cluster spread)`

## Evaluation Metrics
- **SSE (Sum of Squared Errors):** Lower values indicate better clustering.
- **Silhouette Score:** Ranges from -1 to 1; higher values indicate well-separated clusters.

## Future Work
- Expand to hierarchical clustering for comparison.
- Incorporate deep learning methods for better feature extraction.
- Automate cluster selection using adaptive thresholds.

## How to Run
```sh
# Install dependencies
pip install -r requirements.txt

# Run clustering script
python scripts/fractal_clustering.py
```

## Visualization
After running the script, visualize and analyze results using:
```python
import matplotlib.pyplot as plt
plt.show()
```

---
This project provides a structured approach to **fractal clustering**, ensuring meaningful data segmentation. 🚀
