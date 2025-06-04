# 🗳️ VotePulse: Predicting Electoral Outcomes from Campaign Finance and Sentiment

## Project Overview

**VotePulse** is a predictive modeling project focused on U.S. election outcomes using campaign finance data, with future extensions into social media sentiment. The goal is to classify candidates into high or low campaign funding categories and lay the groundwork for a combined sentiment-finance modeling framework to enhance electoral prediction.

## Objectives

- Explore the impact of financial metrics (e.g., cash on hand, disbursements) on campaign success.
- Build and evaluate classification models such as Logistic Regression, Random Forest, and XGBoost.
- Prepare for integration of social media sentiment analysis for a hybrid prediction system.

## Dataset Summary

| Source | Description |
|--------|-------------|
| `elections-2025.csv` | Candidate-level campaign finance data |
| `GOVSTIMESERIES.csv` | Federal financial and demographic trends |
| `United States September 2024 Dataset for website codebook.xlsx` | Metadata for structured reference |
| `xgboost_feature_importance.csv` | Feature importance output from XGBoost |
| `votepulse.Rmd` | Main analysis and modeling script |
| `VotePulse_Presentation.pptx` | Project slide deck |
| `Milestone 2.docx`, `Milestone 3.docx` | White papers documenting process and findings |

## Technologies Used

- **Language**: R (via RMarkdown)
- **Libraries**: `dplyr`, `ggplot2`, `randomForest`, `xgboost`, `caret`
- **Modeling**: Logistic Regression, Random Forest, XGBoost
- **Visualization**: Feature importance plots, confusion matrices

## Methodology

1. **Data Preprocessing**
   - Cleaned numeric fields (removed symbols, converted to numeric)
   - Handled missing data and created binary classification target

2. **Model Training**
   - Split data into training/testing sets
   - Tuned hyperparameters for Random Forest and XGBoost
   - Evaluated models using accuracy, precision, recall, and F1-score

3. **Feature Analysis**
   - Identified top financial predictors (`cash_on_hand`, `disbursements`)
   - Compared model interpretability and performance

## Key Results

- **XGBoost** achieved the highest classification accuracy.
- **Random Forest** showed robust feature importance rankings.
- **Party affiliation** alone had limited predictive power; financial metrics dominated.
- Models were validated using holdout sets and confusion matrix diagnostics.

## Future Enhancements

- Integrate **Twitter/X API** for real-time public sentiment.
- Conduct **sentiment analysis** using NLP libraries like `syuzhet` or `textdata`.
- Deploy an interactive dashboard to track predictions and feature influence.

## Ethical Considerations

- No personal identifiers or sensitive demographic data used.
- Plan to audit model fairness across political affiliations and geographic regions.
- Follows FEC guidelines and open data licensing terms.

## How to Reproduce

1. Clone the repo:
   ```bash
   git clone https://github.com/bobga-herman/Data-science-projects.git
   cd pj_3_vote_pulse
