# Sowing-Success-How-Machine-Learning-Helps-Farmers-Select-the-Best-Crops

# Overview/Introduction

Farmers face the challenge of selecting the best crops to plant each season to maximize yield. Soil condition, measured by metrics such as nitrogen (N), phosphorous (P), potassium (K), and pH levels, plays a crucial role in determining the optimal crop for a field. However, measuring these metrics can be expensive and time-consuming. This project uses machine learning to build a multi-class classification model that predicts the best crop based on soil measurements, helping farmers make data-driven decisions.

# Objectives

1. Build a multi-class classification model to predict the optimal crop based on soil measurements.
2. Identify the most important soil feature for predicting crop type.
3. Provide actionable insights to help farmers select the best crops for their fields.

# Data Source

The dataset, soil_measures.csv, contains the following columns:
  - N: Nitrogen content ratio in the soil.
  - P: Phosphorous content ratio in the soil.
  - K: Potassium content ratio in the soil.
  - pH: pH value of the soil.
  - crop: The optimal crop for the field (target variable).

Each row represents soil measurements for a specific field and the corresponding optimal crop.

# Tools Used

- Python Libraries: Pandas, Scikit-learn
- Modeling: Logistic Regression for multi-class classification.
- Evaluation Metrics: F1 score to assess model performance.
- Data Splitting: Train-test split for model validation.

# Insights

1. Feature Importance:
    - Potassium (K) is the most important feature for predicting the optimal crop, with an F1 score of 0.257.
    - Nitrogen (N) and phosphorous (P) also contribute to the model but with lower predictive power.
    - pH has the least predictive power among the features.
  
      ![d7](https://github.com/user-attachments/assets/edf6f062-1481-4b9d-870a-7878d318e004)

2. Model Performance:
    - The logistic regression model was trained and evaluated using individual features to determine their predictive performance.
    - The F1 score was used to evaluate the model, as it balances precision and recall for multi-class classification.

# Recommendations

1. Focus on Potassium Levels:
    - Farmers should prioritize measuring potassium levels in their soil, as it is the most important factor for crop selection.
2. Soil Testing:
    - While potassium is the most predictive feature, farmers should also consider measuring nitrogen and phosphorous levels for a more comprehensive soil analysis.
3. Model Improvement:
    - Explore more advanced machine learning models (e.g., Random Forest, Gradient Boosting) to improve predictive accuracy.
4. Data Collection:
    - Collect additional soil metrics (e.g., organic matter, moisture levels) to enhance the model's predictive power.

# How to Use This Repository

1. Clone the repository.
2. Install the required Python libraries (pandas, scikit-learn).
3. Run the Jupyter Notebook (Predictive Modeling for Agriculture.ipynb) to reproduce the analysis.
4. Explore the dataset and modify the code to test additional models or features.
