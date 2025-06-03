# ✈️ Flight Delay Prediction Using Machine Learning

This project aims to develop a machine learning model capable of predicting flight delays based on historical flight and weather data. Accurate predictions help airlines reduce disruptions and improve scheduling efficiency, while also enhancing passenger experience.

---

## 🧠 Project Summary

Flight delays pose major challenges in aviation, causing financial losses and customer dissatisfaction. This project uses supervised machine learning techniques—specifically Random Forest and XGBoost—to forecast delays using features from flight logs and weather reports.

---

## ❓ Research Questions

- What are the key factors influencing flight delays?
- How accurately can ML models predict delays using historical and real-time data?
- Which algorithms perform best in terms of precision and recall?

---

## 📊 Data Sources

- [U.S. Department of Transportation - BTS](https://www.transtats.bts.gov/)
- [Kaggle Flight Delay Datasets (2019–2023)](https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023)

### 🧹 Preprocessing Steps

- Missing value imputation (mean strategy)
- Feature engineering: `high_severity_delay` (>30 min delay)
- Normalization of continuous features
- Class balancing considerations

---

## 🧪 Models Used

| Model        | Purpose               | Notes |
|--------------|------------------------|-------|
| Random Forest | Classification of delay severity | Strong performance, ensemble-based |
| XGBoost       | Gradient Boosting Classifier | Captures non-linear patterns well |

Both models achieved **100% accuracy**, but due to **class imbalance**, real-world generalization may differ.

---

## 📈 Evaluation Metrics

- Accuracy
- Confusion Matrix
- ROC Curve (AUC = 1 for both models)

---

## 🖼️ Key Visuals

- **ROC Curve (Random Forest and XGBoost)**
- **Confusion Matrix**
- Visual comparison of delay predictions vs actuals

---

## ⚖️ Ethical Considerations

- **Privacy:** Data is anonymized; no PII used.
- **Fairness:** Care taken to avoid biases by route, airline, or weather condition.
- **Operational Impact:** Misclassification could misinform airline responses—extensive validation recommended.

---

## ✅ Recommendations

- Implement **k-fold cross-validation**
- Use **SMOTE** to address class imbalance
- Tune hyperparameters with grid/random search
- Explore deployment in real-time systems

---

## 🚀 Future Applications

- Airline scheduling optimization
- Airport resource allocation
- Customer service alert systems

---

## 📁 Files Included

- `flight_delay.Rmd` — RMarkdown analysis and model training
- `flight_delay.pdf` — Final white paper
- `README.md` — Project summary for GitHub

---

## 📚 References

- U.S. Department of Transportation (BTS). [Link](https://www.transtats.bts.gov/)
- Kaggle: [Flight Delay & Cancellation Dataset](https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023)

---

© 2025 Bobga-Herman Gwanvoma | Bellevue University | DSC 680 – Applied Data Science
