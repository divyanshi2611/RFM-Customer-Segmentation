# 📊 RFM Customer Segmentation with K-Means

This project performs **customer segmentation** using **Recency, Frequency, Monetary (RFM)** analysis and **K-Means clustering**, based on the [Online Retail dataset](https://www.kaggle.com/datasets/vijayuv/onlineretail?resource=download).

---

## 📂 Project Structure

RFM-Customer-Segmentation

│

├── rfm_segmentation.ipynb # Jupyter notebook with the full pipeline

├── .gitignore

└── .venv # Virtual environment (optional)

## 🔍 Overview

1. Extracts behavioral customer metrics (**RFM**)
2. Normalizes data, determines the **optimal number of clusters** (Elbow Method)
3. Applies **K-Means** to segment customers into meaningful groups
4. Creates **visualizations** (scatter plots, boxplots) for insights

---

## ⚙️ Tech Stack
![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-Matrix%20Computations-lightblue?logo=numpy)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikitlearn)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-yellow?logo=plotly)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-teal?logo=seaborn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

---

## 🚀 How to Use

**1. Clone the repository**

```bash
git clone https://github.com/divyanshi2611/RFM-Customer-Segmentation.git
cd RFM-Customer-Segmentation
```
---
**2. Install dependencies**

Create and activate a virtual environment (recommended):
```bash

python -m venv .venv
source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
pip install pandas numpy matplotlib seaborn scikit-learn notebook
```
---
**3. Download the dataset**

Download OnlineRetail.csv from Kaggle and place it in the project folder.
---
**4. Run the analysis pipeline**

```bash
jupyter notebook rfm_segmentation.ipynb
```
---
**5. Explore**

Data preprocessing
RFM calculation
Clustering results
Visualizations

**Expected Outputs**

RFM features:

**Recency** = Days since last purchase

**Frequency** = Number of purchases

**Monetary** = Total spending

**Elbow plot**: Helps choose number of clusters

**Cluster assignments**: Groups customers (loyal, at-risk, new, etc.)

**Visualizations**: Scatter plots & boxplots for each cluster

---

## 📈 Results & Visualizations

### Elbow Method (Optimal Clusters)
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/49528b7d-179f-4549-9f69-753a713260ba" />

### Customer Segments (K-Means Clusters)
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/fa981197-0771-4ac6-81ea-c453a91fe4d7" />

### Boxplots of RFM Features
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/97f0bb2d-baff-4d50-a0d0-987b75dac6da" />

## Insights

**1️⃣ RFM Distribution by Cluster (Boxplots)**

Cluster 2 has customers with the highest Monetary value and lowest Recency, meaning they are your most loyal and profitable customers.

Cluster 1 has customers with high Recency but low Frequency and Monetary, indicating inactive or churned customers.

Cluster 0 represents moderate Frequency and low Monetary, possibly occasional buyers.

Cluster 3 contains a small group with high Frequency but relatively low Monetary, suggesting frequent low-value buyers.

**2️⃣ Elbow Method (Optimal Number of Clusters)**

The elbow curve shows a sharp decline in WCSS until k=4, after which the reduction flattens.

This indicates that 4 clusters is the optimal choice for customer segmentation, balancing accuracy and simplicity.

**3️⃣ Customer Segmentation Scatter Plot (RFM Clusters)**

The scatter plot clearly separates customers into 4 clusters based on Recency and Monetary value.

Cluster 2 stands out as high-value customers with high spending.

Cluster 1 contains inactive/churned customers (high Recency, low Monetary).

Cluster 0 are average-value customers with low Recency and moderate spend.

Cluster 3 includes frequent but low-spending customers.



