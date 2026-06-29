# 📈 A Multifractal and Regime-Based Forecasting Framework for Brent Crude and BDTI Returns

> **Hybrid financial time series forecasting using Multifractal Detrended Fluctuation Analysis (MF-DFA), market regime detection, and ensemble machine learning models.**

---

## 📖 Overview

Financial markets exhibit nonlinear, non-stationary, and regime-dependent behavior, making accurate forecasting a challenging task.

This project presents a hybrid forecasting framework that combines **multifractal analysis**, **market regime detection**, and **ensemble machine learning models** to predict **next-day Brent Crude Oil returns** using historical Brent Crude prices and the Baltic Dirty Tanker Index (BDTI).

The implementation was developed as part of my **Integrated MSc in Data Science thesis** and investigates the effectiveness of multifractal features across different market regimes.

---

## 🎯 Objectives

- Forecast next-day Brent Crude Oil returns.
- Extract multifractal characteristics using MF-DFA.
- Detect structural market regimes using Binary Segmentation.
- Engineer predictive features from Brent returns, BDTI returns, and multifractal spectrum width (Δα).
- Compare traditional statistical models with modern machine learning approaches.
- Evaluate forecasting performance across different market conditions.

---

## 🔄 Project Workflow

```text
Raw Brent Crude & BDTI Data
            │
            ▼
     Data Cleaning
            │
            ▼
  Log Return Computation
            │
            ▼
 Exploratory Data Analysis
            │
            ▼
 Rolling Volatility Analysis
            │
            ▼
 MF-DFA (Multifractal Analysis)
            │
            ▼
 Rolling Δα Computation
            │
            ▼
 Binary Segmentation
 (Market Regime Detection)
            │
            ▼
 Feature Engineering
            │
            ▼
 Machine Learning Models
            │
            ▼
 Performance Evaluation
            │
            ▼
 Regime-wise Analysis
```

---

## 🤖 Models Implemented

### Machine Learning Models

- Random Forest
- XGBoost
- LightGBM
- CatBoost
- Linear Regression

### Statistical Models

- ARIMA
- GARCH

---

## 📊 Feature Configurations

Three progressively enriched feature sets were evaluated.

| Model | Features |
|--------|----------|
| Model A | Brent Return Lag₁ |
| Model B | Brent Return Lag₁ + BDTI Return Lag₁ |
| Model C | Brent Return Lag₁ + BDTI Return Lag₁ + Multifractal Spectrum Width (Δα) Lag₁ |

---

## 📈 Evaluation Metrics

Model performance is evaluated using

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)

---

## 🛠 Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- SciPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- Ruptures
- XGBoost
- LightGBM
- CatBoost

---

## 📂 Repository Structure

```text
multifractal-regime-forecasting-for-crude-oil/

│
├── data/
│
├── docs/
│   ├── thesis_report.pdf
│   └── research_manuscript.pdf
│
├── images/
│
├── notebook/
│   └── multifractal_regime_forecasting.ipynb
│
├── requirements.txt
│
├── .gitignore
│
└── README.md
```

---

## 🚀 Getting Started

Clone the repository

```bash
git clone https://github.com/Lek0007/multifractal-regime-forecasting-for-crude-oil.git
```

Move into the project directory

```bash
cd multifractal-regime-forecasting-for-crude-oil
```

Install the dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```text
notebook/multifractal_regime_forecasting.ipynb
```

Run all cells sequentially.

---

## 📁 Dataset

This project uses

- Brent Crude Oil historical prices
- Baltic Dirty Tanker Index (BDTI)

The data used in this repository is intended for academic and research purposes.

---

## 📄 Research Documentation

The repository includes

- MSc Thesis Report
- Research Manuscript (Unpublished)

Both documents describe the complete methodology, experiments, and findings.

---

## 📌 Key Highlights

- Hybrid forecasting framework combining multifractal analysis and machine learning.
- Market regime detection using Binary Segmentation.
- Rolling MF-DFA feature extraction.
- Ensemble learning with multiple tree-based algorithms.
- Regime-wise forecasting performance evaluation.
- Comparative analysis against traditional statistical forecasting models.

---

## 🔮 Future Improvements

Potential extensions include

- Deep Learning models (LSTM, GRU, Transformer)
- Attention-based forecasting
- Real-time prediction pipeline
- Explainable AI (SHAP/LIME)
- Hyperparameter optimization using Bayesian Optimization
- Deployment as an interactive dashboard

---

## 👨‍💻 Author

**L V**

Integrated MSc Data Science

GitHub: https://github.com/Lek0007

---

## ⭐ If you found this project useful, consider giving it a star!
