# 📊 RFM Customer Segmentation with K-Means

This project performs **customer segmentation** using **Recency, Frequency, Monetary (RFM)** analysis and **K-Means clustering**, based on the [Online Retail dataset](https://www.kaggle.com/datasets/vijayuv/onlineretail?resource=download).

---

## 📂 Project Structure

RFM-Customer-Segmentation/
│
├── rfm_segmentation.ipynb # Jupyter notebook with the full pipeline
├── .gitignore
└── .venv/ # Virtual environment (optional)

yaml
Copy
Edit

---

## 🔍 Overview

1. Extracts behavioral customer metrics (**RFM**)
2. Normalizes data, determines the **optimal number of clusters** (Elbow Method)
3. Applies **K-Means** to segment customers into meaningful groups
4. Creates **visualizations** (scatter plots, boxplots) for insights

---

## 🚀 How to Use

### 1. Clone the repository
```bash
git clone https://github.com/divyanshi2611/RFM-Customer-Segmentation.git
cd RFM-Customer-Segmentation
2. Install dependencies
Create and activate a virtual environment (recommended):

bash
Copy
Edit
python -m venv .venv
source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
pip install pandas numpy matplotlib seaborn scikit-learn notebook
3. Download the dataset
Download OnlineRetail.csv from Kaggle and place it in the project folder.

4. Run the analysis pipeline
bash
Copy
Edit
jupyter notebook rfm_segmentation.ipynb
5. Explore
Data preprocessing

RFM calculation

Clustering results

Visualizations

📈 Expected Outputs
RFM features:

Recency = Days since last purchase

Frequency = Number of purchases

Monetary = Total spending

Elbow plot → helps choose number of clusters

Cluster assignments → groups customers (loyal, at-risk, new, etc.)

Visualizations → Scatter plots & boxplots for each cluster
