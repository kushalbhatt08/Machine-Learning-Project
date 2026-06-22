# MNIST Binary Classification — Digits 1 vs 7

A machine learning project that builds and compares binary classifiers on a subset of the MNIST dataset (digits 1 and 7), with clustering analysis to explore writing style variations.

---

## Dataset

- **Source:** MNIST subset — digits 1 and 7 only
- **Training set:** 100 images (50 per class)
- **Test set:** 1000 images (100 digit 1s, 900 digit 7s)
- **Image size:** 28×28 pixels (grayscale), flattened to 784 features
- **Preprocessing:** Pixel normalization (÷255) + flattening

---

## Models

### Linear SVM
- Kernel: Linear
- Best C: `0.1` (tuned via 5-fold stratified cross-validation)
- Chosen for its strength in high-dimensional, small-sample settings

### K-Nearest Neighbours (KNN)
- Best k: `1`, Distance metric: Euclidean
- Tuned across k = 1–30 and two distance metrics (Euclidean vs Manhattan)

---

## Results

| Metric | Linear SVM | KNN |
|--------|-----------|-----|
| Accuracy | 0.9420 | 0.9430 |
| F1 Score | 0.9667 | 0.9673 |
| Precision | 1.0000 | 0.9988 |
| Recall | 0.9356 | 0.9378 |
| ROC AUC | 0.9876 | 0.9639 |

SVM is the stronger overall model — perfect precision and significantly better ROC AUC (0.9876 vs 0.9639), meaning more reliable confidence scores across all thresholds.

---

## Clustering Analysis

K-Means clustering applied to 900 digit 7 test samples to discover writing style variation.

- Optimal clusters: **k = 8** (elbow method + silhouette score)
- Each cluster represents a distinct writing style:

| Cluster | Samples | Style |
|---------|---------|-------|
| 1 | 90 | Classic thick-stroked 7 |
| 2 | 130 | Compact, curved diagonal |
| 3 | 106 | Flat top, sharp 90° corner |
| 4 | 119 | Tall narrow, formal/printed |
| 5 | 90 | European style with crossbar |
| 6 | 156 | Bold, wide strokes (most common) |
| 7 | 93 | Curved diagonal, high variation |
| 8 | 116 | Small, thin, quickly written |

---

## Tech Stack

- Python 3.x
- scikit-learn
- NumPy
- Matplotlib / Seaborn
- Jupyter Notebook

---

## Getting Started

```bash
git clone https://github.com/kushalbhatt08/Machine-Learning-Project.git
cd Machine-Learning-Project
pip install -r requirements.txt
jupyter notebook notebooks/machine_learning_01.ipynb
```

---

## Author

**Kushal Bhatt**
GitHub: https://github.com/kushalbhatt08
