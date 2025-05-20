# 📈 Startup Business Profit Prediction

A machine learning-based web application that predicts startup profitability using R&D spend, administration, marketing, and state-wise data input.

## 🧠 Overview

This project aims to predict the profit of a startup based on various input features like R&D Spend, Administration, Marketing Spend, and State. It uses machine learning algorithms trained on the `50_Startups.csv` dataset and is deployed via a simple Flask web application.

---

## 🔍 Features

- Predict startup profit from user input
- Trained using supervised ML algorithms
- Web interface for user-friendly predictions
- Includes one-hot encoded state variables
- Scalable and modular code structure

---

## 🛠️ Tech Stack

- **Python**
- **Pandas, NumPy, Scikit-Learn**
- **Flask** (for deployment)
- **HTML/CSS/Bootstrap** (for frontend)
- **Matplotlib / Seaborn** (for EDA, optional)

---

## 📊 Dataset: `50_Startups.csv`

The dataset consists of the following columns:
- `R&D Spend`
- `Administration`
- `Marketing Spend`
- `State` (California, Florida, New York)
- `Profit` (target variable)

> Categorical feature `State` is one-hot encoded into:
> - `state_florida`
> - `state_new york`
> *(implying California is the base case)*

---

## 📂 About `columns.json`

The `columns.json` file stores the list of input features expected by the model after preprocessing:
```json
{
  "data_columns": [
    "r&d spend",
    "administration",
    "marketing spend",
    "state_florida",
    "state_new york"
  ]
}


