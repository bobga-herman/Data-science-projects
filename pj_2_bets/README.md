# Predicting Sports Betting Outcomes

## Overview

This project applies machine learning techniques to predict potentially profitable bets in the context of soccer match outcomes. The main focus is determining the likelihood of a home team winning a match based on historical game data. By leveraging the Random Forest algorithm, we aim to enhance decision-making in sports betting.

## Problem Statement

Traditional sports betting heavily relies on intuition, expert analysis, and historical trends. However, with the availability of rich datasets and machine learning tools, it is now possible to develop models that learn from past games to predict match results. This project seeks to answer:

- Can we accurately predict the outcome of soccer matches using historical data?
- How impactful is the goal difference metric in determining match outcomes?
- How can these insights be used to improve betting strategies?

## Data

The dataset includes historical soccer match data with key variables such as:

- Home team goals (`hgoal`)
- Visitor team goals (`vgoal`)
- Season
- Derived variables:
  - `GoalDifference`: Difference between home and visitor goals
  - `HomeWin` and `VisitorWin`: Binary outcome indicators

The data was split into an 80% training and 20% testing set for model evaluation.

## Methodology

- **Model Used**: Random Forest Classifier
- **Target Variable**: `HomeWin` (1 for home team win, 0 otherwise)
- **Feature**: `GoalDifference`
- **Evaluation Metrics**:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - Confusion Matrix

## Key Results

- **Accuracy**: 100%
- **Precision**: 100%
- **Recall**: 100%
- **F1-Score**: 100%

> These results are based on a model trained using only `GoalDifference`, and indicate overfitting. Incorporating more features is recommended.

## Visualizations

- Scatter plot: GoalDifference vs HomeWin
- Histogram: GoalDifference distribution
- Feature Importance: Mean Decrease Gini
- Time Series: Home win rate across seasons
- Confusion Matrix Bar Chart

## Conclusions

- **GoalDifference** is a strong predictor of home team victories.
- The model performed exceptionally well but risks overfitting due to reliance on a single feature.
- More complex models including player stats, betting odds, and injuries could improve predictive power and generalizability.

## Future Work

- Integrate additional features like player performance, betting odds, and team form.
- Apply the model to other sports (e.g., basketball, football).
- Use cross-validation and regularization to reduce overfitting.

## Ethical Considerations

This model should be used to **inform** betting decisions, not guarantee profits. Promoting responsible gambling is essential, and models must be regularly evaluated and updated to ensure ethical deployment.

## References

- [Teey2flow, 2020. *How AI and data analytics are revolutionizing sports betting decisions*. Medium](https://medium.com/@teey2flow/how-ai-and-data-analytics-are-revolutionizing-sports-betting-decisions-c5571b63dbc1)
- [Jumbabet. *Understanding season trends: How history affects sports betting*](https://www.jumbabet.com/casino/blog/understanding-season-trends-how-history-affects-sports-betting)
- [Kaggle Dataset: Football Prediction from End Score Dataset](https://www.kaggle.com/datasets/deepak95/footballpredictionfromendscore?select=data_v1.csv)

## Author

**Bobga-Herman Gwanvoma**  
Bellevue University – DSC 680 – Applied Data Science  
April 2025
