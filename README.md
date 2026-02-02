# 🏀 NBA Player Performance Analysis & Modeling

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?logo=scikit-learn)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?logo=sqlite)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)
![Status](https://img.shields.io/badge/Project-Portfolio-success)

End-to-end **data science project** analyzing historical NBA data to engineer player features, explore performance trends, and build predictive models for scoring outcomes.

This project demonstrates practical skills in:

- Data engineering (SQL → features)
- Feature engineering from event-level data
- Exploratory Data Analysis (EDA)
- Visualization
- Machine learning modeling
- Reproducible pipelines

---

## 🚀 Project Highlights

- Processed **65k+ NBA games** from a 2GB SQLite database
- Engineered **player-level features** from play-by-play events (points, rebounds, context)
- Built **analysis-ready dataset** for modeling
- Trained **Logistic Regression & Random Forest**
- Achieved **ROC-AUC ≈ 0.69 baseline**
- Identified class imbalance & feature limitations as key bottlenecks

---

## 📦 Dataset

NBA historical database from Kaggle  
https://www.kaggle.com/datasets/wyattowalsh/basketball

### Setup
1. Download dataset
2. Place file at `data/raw/NBA.sqlite`
3. Run notebooks sequentially

---

## 📁 Repository Structure

```
data/
 ├── raw/           # SQLite database (not tracked)
 └── processed/     # Engineered features

notebooks/
 ├── 01_eda.ipynb        # Feature engineering
 ├── 02_analysis.ipynb   # Visualization & insights
 └── 03_modeling.ipynb   # ML models & evaluation

figures/            # Saved charts
src/                # Helper scripts
```

---

## 🧠 Workflow

### 01 — Feature Engineering
- Extract scoring & rebound events
- Aggregate player stats per game
- Merge season context
- Export modeling-ready table

### 02 — Analysis
- Player comparisons
- Distribution analysis
- Seasonal trends
- Regular vs playoff performance

### 03 — Modeling
- Target: predict **20+ point games**
- Logistic Regression baseline
- Random Forest benchmark
- ROC-AUC, confusion matrix, class imbalance analysis

---

## 🛠️ Tech Stack

Python • Pandas • NumPy • Matplotlib • Seaborn • scikit-learn • SQLite • Jupyter

---

## 📈 Future Improvements

- Rolling averages & advanced stats
- Minutes played / shot attempts
- Class balancing (SMOTE / weights)
- Gradient boosting models (XGBoost / LightGBM)
- Time-series validation

---


## 👤 Author

Data science portfolio project showcasing applied analytics and machine learning skills on real-world sports data.
