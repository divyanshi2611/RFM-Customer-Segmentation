📊 RFM Customer Segmentation with K-Means
This project performs customer segmentation using Recency, Frequency, Monetary (RFM) analysis and K-Means clustering based on the Online Retail dataset available on Kaggle (https://www.kaggle.com/datasets/vijayuv/onlineretail?resource=download).

📂 Project Structure
RFM-Customer-Segmentation/
│
├── rfm_segmentation.ipynb   # Jupyter notebook with the full pipeline
├── .gitignore
└── .venv/                   # Virtual environment (optional)

🔍 Overview

1) Extracts behavioral customer metrics (RFM)
2) Normalizes data, determines the ideal number of clusters via the Elbow Method
3) Applies K-Means to segment customers into meaningful groups
4) Visualizes segmentation results with scatter plots and boxplots

🚀 How to Use

1) Clone the repository

git clone https://github.com/divyanshi2611/RFM-Customer-Segmentation.git
cd RFM-Customer-Segmentation

2) Install dependencies
Create and activate a virtual environment (recommended):

python -m venv .venv
source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
pip install pandas numpy matplotlib seaborn scikit-learn notebook

3) Download the dataset
Download OnlineRetail.csv from Kaggle and place it into the project folder.

4) Run the analysis pipeline
Launch the Jupyter notebook:

jupyter notebook rfm_segmentation.ipynb


Explore step-by-step: Preprocessing, RFM calculation, clustering, and visualizations.

📈 Expected Outputs

RFM features: Recency (days since last purchase), Frequency (# of purchases), Monetary (total spending)
Elbow plot: Helps choose cluster size
Cluster assignments: Each customer is assigned to a cluster (e.g., loyal customers, at-risk customers, new customers)
Visualizations: Scatter plots and boxplots to analyze cluster characteristics
