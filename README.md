# Zoo Animal Clustering 🦁

An unsupervised machine learning project that clusters 101 zoo animals 
into groups based on biological traits — without using any labels.

## 📌 Objective
To discover whether K-Means clustering can reconstruct biological animal 
taxonomy (mammal, bird, fish, etc.) purely from physical trait data.

## 📊 Dataset
- **Source:** [Zoo Dataset – Kaggle](https://www.kaggle.com/datasets/raghunathangrdr/zoo-data-dataset)
- 101 animals, 16 binary/numeric features (hair, feathers, eggs, legs, etc.)

## 🛠️ Techniques Used
- Exploratory Data Analysis (EDA)
- Feature Standardization (StandardScaler)
- K-Means Clustering
- Principal Component Analysis (PCA) for 2D visualization
- Hierarchical Clustering (Dendrogram)
- Silhouette Score evaluation

## 📈 Key Results
- K-Means with k=7 clusters closely mirrors the 7 biological animal classes
- PCA scatter plot shows clear cluster separation
- Heatmap of cluster trait profiles reveals interpretable groupings

## 🧰 Libraries
`pandas` `numpy` `scikit-learn` `matplotlib` `seaborn` `scipy`

## 🚀 How to Run
1. Clone this repo
2. Open `zoo-data-analysis.ipynb` in Jupyter or VS Code
3. Download the dataset from the Kaggle link above and place it in `/input/`
4. Run all cells
