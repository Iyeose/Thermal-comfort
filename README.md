# Data-Driven Prediction of Human Thermal Comfort

This project explores the use of machine learning approaches to predict human thermal comfort more accurately than traditional models such as the Predicted Mean Vote (PMV) or Adaptive Comfort models. It leverages the ASHRAE Global Thermal Comfort Database II (100k+ entries) and applies modern data science methods to identify the key drivers of human comfort in built environments.

🎯 ## Objectives

Evaluate the performance of multiple ML models (Logistic Regression, SVM, Random Forest, XGBoost, Deep Neural Networks) for predicting thermal sensation.

Handle data preprocessing challenges: missing values, class imbalance (via SMOTE), and feature engineering.

Optimize model performance through hyperparameter tuning.

Analyze feature importance to understand which environmental, personal, and contextual factors most influence thermal comfort.

📊 ## Dataset

Source: ASHRAE Global Thermal Comfort Database II

### Variables:

Environmental: operative temperature, humidity, air velocity, etc.

Personal: clothing insulation, metabolic rate, age, sex.

Contextual: season, building type, cooling strategy, Köppen climate classification.

Target: Thermal sensation votes on a 7-point ASHRAE scale (-3 = Cold to +3 = Hot).

🛠️ ## Methods

Preprocessing: Missing data imputation, feature pruning, and normalization.

Balancing: Synthetic Minority Oversampling (SMOTE).

### Modeling:

Logistic Regression (baseline)

Support Vector Machine (SVM)

Random Forest

Extreme Gradient Boosting (XGBoost)

Deep Neural Network (Keras/TensorFlow)

Evaluation: Accuracy, Precision, Recall, F1-score, Confusion Matrices.

🚀 ## Results

Baseline Logistic Regression: 23% accuracy.

Best Model (XGBoost, tuned): 53.1% accuracy → a 130% improvement over baseline.

### Key Insights:

Random Forest emphasized physical + personal factors (temperature, age, clothing).

XGBoost emphasized contextual/geographical factors (climate classification).

Both strategies highlight that thermal comfort depends on both immediate environment and broader context.

🌍 ## Impact

Demonstrates that machine learning outperforms traditional comfort models.

Provides actionable insights for energy-efficient HVAC control, personalized comfort systems, and climate-responsive architecture.

Offers a reproducible framework for applying data-driven methods in building science.
