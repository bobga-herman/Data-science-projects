# 🏡 pj_4_housing: Predicting Housing Prices Based on Real Estate Features

## 📌 Overview

This project leverages machine learning techniques to predict housing prices using the Ames Housing dataset. The dataset includes detailed information on over 80 features such as square footage, neighborhood, construction quality, and garage capacity. The goal is to identify the most influential variables and develop an accurate predictive model that can assist buyers, sellers, and real estate professionals.

## 🎯 Objectives

- Identify the key features influencing housing prices.
- Compare the performance of multiple regression models.
- Build a predictive model with high accuracy and interpretability.
- Visualize relationships and model outputs to validate insights.

## 🧾 Dataset

- **Source**: [Ames Housing Dataset - Kaggle](https://www.kaggle.com/datasets/prevek18/ames-housing-dataset)
- **Observations**: 2,930 residential properties
- **Features**: 80+ variables including:
  - `GrLivArea` – Above-ground living area (sqft)
  - `OverallQual` – Overall material and finish quality
  - `Neighborhood` – Location group
  - `GarageCars` – Garage size in car capacity
  - `YearBuilt` – Construction year
  - `SalePrice` – Target variable

## ⚙️ Methods

### Data Preprocessing

- Imputed missing values with domain-specific logic (e.g., neighborhood-wise median for `LotFrontage`).
- Applied **log transformation** to `SalePrice` to normalize distribution.
- Used **one-hot encoding** for categorical features.
- Standardized numeric variables for model stability.

### Models Implemented

- Linear Regression
- Ridge & Lasso Regression
- Decision Tree
- Random Forest
- **XGBoost (Gradient Boosting)** – Best performer

### Model Evaluation Metrics

- **RMSE** (Root Mean Square Error)
- **MAE** (Mean Absolute Error)
- **R² Score** – Best score: **0.91** with XGBoost

## 📊 Key Visualizations

- **Correlation Heatmap** – Highlighted strong linear relationships.
- **Feature Importance Plot** – `GrLivArea`, `OverallQual`, and `Neighborhood` were top predictors.
- **Boxplot by Neighborhood** – Showed price disparity across locations.
- **Actual vs Predicted Scatterplot** – Demonstrated strong predictive alignment.

## 🧠 Results & Insights

- **Top Predictors**: Above-ground living area, overall quality, and neighborhood.
- **Model Performance**: XGBoost achieved the highest accuracy (R² = 0.91).
- **Interpretation**: Buyers prioritize interior size and quality over lot size. Homes in affluent neighborhoods fetch premium prices.

## 🔍 Future Work

- Incorporate macroeconomic indicators (e.g., mortgage rates).
- Explore deep learning techniques for non-linear relationships.
- Conduct temporal trend analysis with time-series extensions.

## 📁 Files

- `AmesHousing.csv` – Dataset
- `milestone_630_final.pdf` – Final white paper
- `Gwanvoma_630_milestone_final_pp.pptx` – Final presentation
- `Gwanvoma_milestone_630_final.docx` – Source document
- `milestone_630_final.Rmd` – Code and analysis in R Markdown

## 👨‍💻 Author

**Bobga-Herman Gwanvoma**  
Bellevue University | DSC 630 – Predictive Analytics  
Instructor: Professor Andrew Hua  
Date: February 28, 2025

