# ✈️ Predicting Flight Delays Using Machine Learning

## 📌 Project Overview
This project develops machine learning models to predict flight delays using historical data, weather conditions, and airline operations. The goal is to help airlines and passengers minimize disruptions and improve planning by anticipating delays before they occur.

## 💼 Business Problem
Flight delays cost the airline industry millions annually and lead to customer dissatisfaction and logistical challenges. By analyzing patterns in flight schedules, weather, and operations, this project aims to predict whether a flight will have a **high-severity delay** (over 30 minutes).

## ❓ Research Questions
- What are the key factors influencing flight delays?
- How accurately can machine learning models predict delays?
- Which algorithm (Random Forest or XGBoost) performs best?

## 📊 Datasets
- **Airline_Delay_Cause.csv**: Operational delay data by airline and airport
- **flights_sample_3m.csv**: Flight-level data (e.g., departure, arrival, delays)
- **Sources**:  
  - [Bureau of Transportation Statistics](https://www.transtats.bts.gov/)
  - [Kaggle Flight Delay Dataset (2019–2023)](https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023)

## 🔧 Methodology
1. **Data Cleaning**:
   - Removed duplicates and merged datasets on `AIRLINE_CODE` and `carrier`
   - Imputed missing values with column means
2. **Feature Engineering**:
   - Created `high_severity_delay` (binary: delay > 30 min)
   - Scaled numerical delay features
3. **Modeling**:
   - **Random Forest**: Trained on a balanced dataset via undersampling
   - **XGBoost**: Gradient boosting for binary classification
4. **Evaluation**:
   - Accuracy, Confusion Matrix, ROC Curve, and AUC

## 📈 Results
- Both Random Forest and XGBoost achieved **100% accuracy** on the test set
- ROC AUC for both models: **1.0**
- Feature importance: Weather, Carrier Delay, and NAS Delay were top predictors

## 📊 Visualizations
- Histograms for delay causes
- Scatter plots for delay correlation
- ROC Curves for both models
- Confusion Matrices

## 💡 Recommendations
- Implement **SMOTE** or oversampling for better class balance
- Use **k-fold cross-validation** to reduce overfitting
- Explore **real-time streaming data** integration for live predictions

## 🛠️ Tools Used
- **Language**: R
- **Libraries**: `dplyr`, `ggplot2`, `randomForest`, `xgboost`, `caret`, `pROC`

## ▶️ How to Run
1. Open `flight_delay.Rmd` in RStudio
2. Extract and load the zipped datasets:
   - `ot_delaycause1_DL.zip`
   - `flights_sample_3m.csv.zip`
3. Execute all chunks to reproduce preprocessing, modeling, and visualizations

## ⚖️ Ethical Considerations
- All data is anonymized
- Fairness across airlines and airports was considered
- False predictions could misguide operations — validation is key

## 📦 Folder Structure

## 📚 References
- U.S. Department of Transportation: [https://www.transtats.bts.gov/](https://www.transtats.bts.gov/)
- Kaggle Flight Delays: [https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023](https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023)
