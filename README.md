# 🏀 NBA Players Performance Analysis & Modeling

📊 This project implements an end-to-end data science workflow on historical NBA data — from raw SQL ingestion and feature engineering to exploratory analysis, visualization, and predictive modeling.

The objective is to extract meaningful insights from player performance and build models that predict scoring outcomes using real game statistics.

This repository is designed as a professional portfolio project, demonstrating practical skills in:

- Data engineering
- Feature engineering
- Exploratory Data Analysis (EDA)
- Statistical visualization
- Machine learning modeling
- Reproducible workflows

---

## 📦 Dataset: NBA Database (Kaggle)

This project uses the **NBA Database** dataset from Kaggle — a comprehensive historical dataset containing professional NBA game and player statistics.

Dataset source:  
https://www.kaggle.com/datasets/wyattowalsh/basketball

### Dataset Overview
- 🏀 30 NBA teams
- 👤 4,800+ players
- 📆 65,000+ games since 1946
- 📊 Play-by-play + box scores
- 📋 Multiple relational SQL tables

This structure enables event-level analytics and player-level modeling.

---

## ⬇️ Data Setup

The raw SQLite database is not included due to size (~2GB).

### Steps
1. Download the dataset from Kaggle
2. Place the file at: `data/raw/NBA.sqlite`
3. Run notebooks sequentially inside the `notebooks/` folder

---

## 🎯 Objectives

- Clean and preprocess raw play-by-play data
- Engineer player-level features (points, rebounds, game context)
- Explore trends across players and seasons
- Visualize performance distributions
- Build predictive models for scoring outcomes (20+ points)
- Evaluate models using ROC-AUC and classification metrics

---

## 📁 Project Structure

```
NBA_players_performance/
│
├── data/
│   ├── raw/           # SQLite database (not tracked)
│   └── processed/     # Engineered feature tables
│
├── notebooks/
│   ├── 01_eda.ipynb        # Feature engineering
│   ├── 02_analysis.ipynb   # Visualization & insights
│   └── 03_modeling.ipynb   # ML models & evaluation
│
├── figures/            # Saved plots
├── src/                # Reusable scripts
└── README.md
```

---

## 🧠 Workflow

### 01 — EDA & Feature Engineering
- Extract scoring events from play-by-play
- Compute player points per game
- Derive rebound counts
- Merge season and game context
- Produce a clean modeling-ready feature table

### 02 — Analysis
- Points distributions
- Player comparisons
- Season trends
- Regular vs playoff performance
- Rebounds exploration as additional signals

### 03 — Modeling
- Target: 20+ points classification
- Logistic Regression baseline
- Random Forest benchmark
- Preprocessing pipelines (encoding + scaling)
- ROC-AUC and confusion matrix evaluation

---

## 📊 Key Results

- Built player-level features directly from raw event data
- Engineered rebounds as additional predictive signals
- Logistic Regression & Random Forest achieved ROC-AUC ≈ **0.69**
- Identified class imbalance as the main modeling challenge
- Demonstrated a complete pipeline from SQL → features → modeling

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- scikit-learn
- SQLite
- Jupyter Notebook

---

## 🚀 Future Work

- Add advanced stats (minutes, shot attempts, efficiency metrics)
- Create rolling averages and recent-form features
- Handle class imbalance (class weights / SMOTE)
- Try Gradient Boosting (XGBoost / LightGBM)
- Perform time-based validation by season
- Deploy model as API or dashboard

---

## 👤 Author

Portfolio project showcasing practical data engineering, analytics, and machine learning skills applied to real-world sports data.



