# 🌸 Iris Flower Classification

A Machine Learning project that predicts the species of an Iris flower based on its physical measurements using Python and Scikit-Learn.

---

## 📌 Project Overview

| Item | Details |
|---|---|
| **Problem Type** | Multi-Class Classification |
| **Dataset** | Iris Dataset (150 samples, 3 species) |
| **Algorithms** | Logistic Regression, Random Forest, Decision Tree |
| **Best Accuracy** | ~97% |
| **Environment** | Google Colab |
| **Language** | Python 3 |

---

## 🎯 Objective

Predict the species of an Iris flower — **Setosa**, **Versicolor**, or **Virginica** — using 4 input features:

- Sepal Length (cm)
- Sepal Width (cm)
- Petal Length (cm)
- Petal Width (cm)

---

## 📁 Project Structure

```
iris-flower-classification/
│
├── iris_classification.ipynb   # Main Colab notebook (full ML pipeline)
├── README.md                   # Project documentation
└── docs/
    └── Iris_Classification_Report.docx  # Full project report
```

---

## 📊 Dataset

- **Source:** [Data Professor GitHub](https://raw.githubusercontent.com/dataprofessor/data/master/iris.csv)
- **Rows:** 150
- **Columns:** 5 (4 features + 1 target)
- **Classes:** 3 species, 50 samples each (perfectly balanced)

---

## 🔁 ML Pipeline

```
Load Dataset → EDA → Preprocess → Train Models → Evaluate → Compare → Predict
```

1. **Load Data** — Read CSV directly from GitHub URL using `pandas`
2. **EDA** — Shape, statistics, missing values, class distribution
3. **Visualizations** — Count plot, Pairplot, Heatmap, Box plots
4. **Preprocessing** — Label Encoding, Train/Test Split (80/20), Feature Scaling
5. **Model Building** — Train 3 classifiers
6. **Evaluation** — Accuracy, Confusion Matrix, Classification Report
7. **Comparison** — Combined results table using `pd.concat`
8. **Prediction** — Static + Interactive user input

---

## 🤖 Models Used

| Model | Training Accuracy | Testing Accuracy |
|---|---|---|
| Logistic Regression | ~97% | ~97% |
| Random Forest | ~97% | ~97% |
| Decision Tree | ~98% | ~93-97% |

---

## 📦 Libraries Used

| Library | Purpose |
|---|---|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` | Plotting charts |
| `seaborn` | Statistical visualizations |
| `scikit-learn` | ML models, preprocessing, evaluation |

---

## 🚀 How to Run

1. Open [Google Colab](https://colab.research.google.com)
2. Upload `iris_classification.ipynb`
3. Click **Runtime → Run All**
4. When prompted in the last cell, enter your flower measurements
5. Get instant species prediction from all 3 models!

---

## 📸 Sample Output

**Model Comparison Table:**
```
   Model                Training Accuracy  Testing Accuracy
0  Logistic Regression  0.9750             0.9667
1  Random Forest        0.9750             0.9667
2  Decision Tree        0.9833             0.9333
```

**Interactive Prediction:**
```
Enter Sepal Length (cm): 5.1
Enter Sepal Width  (cm): 3.5
Enter Petal Length (cm): 1.4
Enter Petal Width  (cm): 0.2

Logistic Regression → Iris-setosa (Confidence: 98%)
Random Forest       → Iris-setosa (Confidence: 99%)
Decision Tree       → Iris-setosa (Confidence: 100%)

🏆 Final Verdict → Iris-setosa (3/3 models agree)
```

---

## 📚 Reference

This project is inspired by the [Data Professor](https://www.youtube.com/@DataProfessor) ML tutorial series. The same pipeline structure (load from URL → split X/y → train/test split → build models → pd.concat comparison) has been adapted and extended for Iris Flower Classification.

---

## 👤 Author

**Vinay Kartheek Bathala** — Submitted For: SRM INSIDERS | SRMIST 2025-26
