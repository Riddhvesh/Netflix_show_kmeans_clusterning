# Netflix_show_kmeans_clusterning
#  Netflix Show Clustering using K-Means

This project uses unsupervised machine learning to group Netflix movies based on their **genre**, **duration**, **rating**, and **release year**.  
We apply **K-Means clustering** to discover patterns in the content and visualize the clusters using **PCA**.


## 🚀 Overview

- 📊 Dataset: [Netflix Movies and TV Shows (Kaggle)](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- 🤖 Model: KMeans Clustering (Unsupervised ML)
- 📉 Visualization: PCA for 2D scatter plot
- 🧹 Preprocessing:
  - Converted duration to numeric
  - Extracted primary genre
  - One-hot encoded categorical columns
  - Scaled all features

---

## 🧠 Objective

To group similar Netflix movies without any labels using K-Means clustering and identify **hidden patterns** among content types such as:

- Are certain genres typically shorter?
- Do some clusters contain mostly old or new movies?
- How are ratings and genres related?

---

## 📁 Features Used

| Feature        | Description                            |
|----------------|----------------------------------------|
| `genre`        | Primary genre extracted from listed_in |
| `duration`     | Movie length in minutes                |
| `rating`       | Age-based rating (e.g., PG, R)         |
| `release_year` | Year the movie was released            |

---

## 📌 Clustering Approach

1. **Preprocess Data**: Clean and filter for only movies, remove nulls, encode categories.
2. **Scale Features**: Standardize features using `StandardScaler`.
3. **Apply KMeans**: Chose optimal `k` using the elbow method.
4. **Visualize**: Reduced to 2D using PCA and plotted with Seaborn.

---

## 📈 Output

Below is the PCA-based cluster visualization:

![Netflix Show Clusters](path-to-your-image.png)

Each point represents a movie, color-coded by its cluster.

---

## 🔍 Example Cluster Insights

| Cluster | Genre           | Duration | Rating | Observation                          |
|---------|------------------|----------|--------|--------------------------------------|
| 0       | Comedies         | ~90 min  | PG     | Light, short, family-friendly movies |
| 1       | Thrillers        | ~120 min | R      | Longer, mature, intense plots        |
| 2       | Documentaries    | ~70 min  | PG-13  | Short, informative content           |
| 3       | Action & Drama   | ~110 min | TV-MA  | High-energy, adult themes            |

---

## 🛠 Tech Stack

- `Python`
- `Pandas`, `NumPy`
- `Scikit-learn` (KMeans, PCA, StandardScaler)
- `Seaborn`, `Matplotlib`

---

