# Zoo Animal Clustering 🦁
> Can an algorithm rediscover biology from scratch?

An unsupervised machine learning project that clusters 101 zoo animals
into biologically meaningful groups — using only physical trait data,
with zero labels.

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange?logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Objective

To discover whether **K-Means clustering** can reconstruct biological
animal taxonomy (Mammal, Bird, Fish, Reptile, Amphibian, Bug,
Invertebrate) purely from 16 physical trait features — with no labels
given to the model.

---

## 📊 Dataset

| Property | Detail |
|---|---|
| Source | [Zoo Dataset – Kaggle](https://www.kaggle.com/datasets/raghunathangrdr/zoo-data-dataset) |
| Animals | 101 |
| Features | 16 (hair, feathers, eggs, fins, legs, etc.) |
| Target | 7 biological classes (used only for validation) |

---

## 🛠️ Techniques Used

| Technique | Purpose |
|---|---|
| EDA + `df.describe()` | Understand data distribution |
| StandardScaler | Normalize features before clustering |
| K-Means (k=7) | Group animals into 7 clusters |
| PCA (2 components) | Visualize 16D data in 2D |
| Hierarchical Clustering | Validate groupings via dendrogram |
| Silhouette Score | Evaluate cluster quality for k=2..9 |

---

## 📈 Key Results

- K-Means with **k=7** closely mirrors the 7 biological animal classes
- The **cluster trait heatmap** shows the model independently discovered
  concepts like "Mammals" (hair=1, milk=1) and "Fish" (fins=1, aquatic=1)
- The **dendrogram** from Hierarchical Clustering independently validates
  K-Means groupings
- **Silhouette Score** analysis confirms k=7 is a well-justified choice

---

## 📁 Project Structure

zoo-animal-clustering/
│
├── zoo-data-analysis.ipynb   # Main analysis notebook
├── requirements.txt          # Python dependencies
├── .gitignore
└── README.md

---

## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/Prasmitprayansu/zoo-animal-clustering.git
cd zoo-animal-clustering

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download the dataset from Kaggle and place the CSV in /input/

# 4. Launch Jupyter
jupyter notebook zoo-data-analysis.ipynb
```

---

## 🔮 Next Steps

- [ ] Add Elbow Method chart alongside Silhouette Score
- [ ] Label key animals on PCA scatter plot
- [ ] Calculate `adjusted_rand_score` vs true class labels
- [ ] Compare with a supervised Random Forest classifier

---

## 🧰 Tech Stack

`Python` `Pandas` `NumPy` `Scikit-learn` `Matplotlib` `Seaborn` `SciPy`
