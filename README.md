# 🧬 Yeast Protein Localization Sites Clustering

## 📌 Project Overview

This project applies **unsupervised machine learning** techniques to cluster yeast proteins based on their biological characteristics. Instead of using protein localization labels during training, the models discover natural groups by analyzing similarities in protein features.

The project implements **K-Means Clustering** and **Agglomerative Clustering**, determines the optimal number of clusters using the **Elbow Method** and **Silhouette Score**, and visualizes clustering results using **Principal Component Analysis (PCA)**.

---

## 🎯 Objectives

- Perform exploratory data analysis on the yeast protein dataset.
- Preprocess and standardize numerical features.
- Determine the optimal number of clusters.
- Apply K-Means Clustering.
- Apply Agglomerative Clustering.
- Compare clustering performance.
- Visualize clusters using PCA.
- Save trained models and clustering results.

---

## 📂 Dataset Information

- **Dataset:** Yeast Protein Localization Dataset
- **Learning Type:** Unsupervised Learning
- **Number of Samples:** 1,484
- **Number of Features:** 8
- **Target Column:** `class` (used only for evaluation and comparison)

### Feature Description

| Feature | Description |
|----------|-------------|
| mcg | McGeoch's method for signal sequence recognition |
| gvh | von Heijne's signal sequence recognition score |
| alm | ALOM membrane-spanning region prediction score |
| mit | Mitochondrial localization score |
| erl | Endoplasmic reticulum localization signal |
| pox | Peroxisomal localization signal |
| vac | Vacuolar localization score |
| nuc | Nuclear localization score |

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SciPy
- Joblib
- Google Colab

---

## 📋 Project Workflow

1. Data Loading
2. Exploratory Data Analysis (EDA)
3. Data Preprocessing
4. Feature Scaling using StandardScaler
5. Elbow Method
6. Silhouette Score Evaluation
7. K-Means Clustering
8. Agglomerative Clustering
9. PCA Visualization
10. Cluster Analysis
11. Save Models and Results

---

## 📊 Results

- **Optimal Number of Clusters:** **4**
- **Best Silhouette Score:** **0.1142**
- Successfully grouped proteins into meaningful clusters using K-Means and Agglomerative Clustering.
- Reduced high-dimensional data into two dimensions using PCA for visualization.

---

## 📈 Visualizations

### Class Distribution

![Class Distribution](images/class_distribution.png)

---

### Elbow Method

![Elbow Plot](images/elbow_plot.png)

---

### Silhouette Score

![Silhouette Score](images/silhouette_score.png)

---

### PCA Cluster Visualization

![PCA Clusters](images/pca_clusters.png)

---

### Agglomerative Clustering

![Agglomerative Clustering](images/agglomerative_clusters.png)

---

## 📁 Repository Structure

```text
Yeast-Protein-Localization-Clustering/
│
├── data/
│   └── yeast_data.csv
│
├── images/
│   ├── class_distribution.png
│   ├── elbow_plot.png
│   ├── silhouette_score.png
│   ├── pca_clusters.png
│   └── agglomerative_clusters.png
│
├── models/
│   ├── kmeans_model.pkl
│   └── scaler.pkl
│
├── notebooks/
│   └── Yeast_Protein_Localization_Clustering.ipynb
│
├── outputs/
│   ├── clustered_yeast.csv
│   └── cluster_centers.csv
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/yashii24/Yeast-Protein-Localization-Clustering.git
```

### 2. Navigate to the project directory

```bash
cd Yeast-Protein-Localization-Clustering
```

### 3. Install the required dependencies

```bash
pip install -r requirements.txt
```

### 4. Open the notebook

Launch the notebook located in the `notebooks` folder using Jupyter Notebook or Google Colab and run all cells.

---

## 📌 Files Included

| File | Description |
|------|-------------|
| `yeast_data.csv` | Original dataset |
| `clustered_yeast.csv` | Dataset with cluster assignments |
| `cluster_centers.csv` | K-Means cluster centers |
| `kmeans_model.pkl` | Trained K-Means model |
| `scaler.pkl` | StandardScaler object |
| `Yeast_Protein_Localization_Clustering.ipynb` | Complete notebook |

---

## 🔮 Future Improvements

- Implement DBSCAN clustering.
- Apply Gaussian Mixture Models.
- Explore additional cluster validation metrics.
- Build an interactive Streamlit application.
- Experiment with advanced dimensionality reduction techniques such as t-SNE and UMAP.

---

## 💡 Skills Demonstrated

- Exploratory Data Analysis
- Feature Scaling
- Unsupervised Machine Learning
- K-Means Clustering
- Hierarchical Clustering
- Principal Component Analysis (PCA)
- Cluster Evaluation
- Data Visualization
- Model Serialization using Joblib
- Google Colab
- Git & GitHub

---

## 👩‍💻 Author

**Yashi Kardam**

If you found this project useful, consider giving it a ⭐ on GitHub.
