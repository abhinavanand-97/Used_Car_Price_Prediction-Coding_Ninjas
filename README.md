# 🚗 Used Car Price Prediction

A beginner machine learning project that predicts the price of used cars using regression models. Built as part of the **Coding Ninjas** curriculum.

---

## 📌 Project Overview

Ever wondered what a used car *should* cost? This project uses real-world car listing data to build a model that estimates the fair price of a used car based on its features — like model year, mileage, horsepower, and accident history.

Two regression models were trained and compared:
- **Linear Regression** — simple and interpretable
- **Random Forest Regressor** — more powerful, ensemble-based

---

## 📂 Dataset

- **File:** `used_cars.csv`
- **Rows:** ~4,009 car listings
- **Features:** 12 columns including brand, model, model year, mileage, fuel type, engine, transmission, exterior/interior color, accident history, clean title, and price

---

## 🛠️ What Was Done

1. **Data Cleaning** — fixed data types, renamed columns, extracted useful info from text fields (e.g., horsepower from engine description, speeds from transmission string)
2. **Handling Missing Values** — used mode for categorical columns, median for numerical ones
3. **Feature Engineering** — created new columns like `horsepower`, `engine_displacement`, `transmission_speeds`, and `is_automatic`
4. **Exploratory Data Analysis (EDA)** — visualized price distribution, feature relationships, and a correlation heatmap
5. **Log Transformation** — applied to price to handle skewness
6. **Label Encoding** — converted categorical columns to numbers for ML compatibility
7. **Model Training** — trained Linear Regression and Random Forest on an 80/20 train-test split
8. **Model Evaluation** — compared models using MAE, RMSE, and R² score
9. **Feature Importance** — identified which features matter most in predicting price

---

## 📊 Results

| Model | R² Score |
|---|---|
| Linear Regression | ~lower |
| **Random Forest** | **~higher ✅ (Best Model)** |

> **Key Finding:** Model year and total miles driven were the strongest predictors of a car's price.

---

## 🧰 Libraries Used

```
numpy
pandas
matplotlib
seaborn
scipy
scikit-learn
```

---

## 🚀 How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scipy scikit-learn
   ```
3. Place `used_cars.csv` in the same directory as the notebook
4. Open and run `Used_Car_Price_Prediction.ipynb` in Jupyter Notebook or Google Colab

---

## 👤 About

This is my **first machine learning project** — built while learning data science from scratch through Coding Ninjas. Feedback and suggestions are always welcome! 🙌
