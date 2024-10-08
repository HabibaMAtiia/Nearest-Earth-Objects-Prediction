# Nearest-Earth-Objects-Prediction
## Project Overview
In this project, we analyze a real-world dataset tracking 338,199 Near-Earth Objects (NEOs) observed by NASA between 1910 and 2024. The goal is to develop a machine learning model that can accurately predict whether a NEO poses a potential hazard to Earth, as indicated by the "is_hazardous" classification. Accurately identifying dangerous NEOs is crucial for planetary defense and ensuring preparedness for potential threats. The project will involve data preprocessing, feature selection, and model training to classify NEOs based on their proximity and characteristics.
## Problem Statement
Our task is to predict whether a NEO is hazardous based on its characteristics. This classification is critical for planetary defense strategies.
## Dataset
Dataset contains 338,200 records. Its features includes:
1. neo_id: Unique Identifier for each Asteroid
2. name: Name given by NASA
3. absolute_magnitude: Describes intrinsic luminosity
4. estimated_diameter_min: Minimum Estimated Diameter in Kilometers
5. estimated_diameter_max: Maximum Estimated Diameter in Kilometers
6. orbiting_body: Planet that the asteroid orbits
7. relative_velocity: Velocity Relative to Earth in Kmph
8. miss_distance: Distance in Kilometres missed
9. is_hazardous: Boolean feature that shows whether asteroid is harmful or not
## Objectives
- Clean and preprocess the dataset.
- Perform exploratory data analysis to gain insights into NEO characteristics.
- Train and evaluate multiple machine learning models to classify NEOs as hazardous or non-hazardous.
- Use evaluation metrics such as accuracy, precision, recall, and F1-score to assess model performance.
## Installation
- Install the required dependencies:
  - pip install -r requirements.txt
## Data Preprocessing
- Missing data was handled by imputation or removal.
- Outliers was handled by IQR technique.
- Features was scaled using MinMaxScaler for model compatibility.
- Categorical features were encoded for machine learning model input.
- Handling Imbalanced Classes by Oversampling technique (SMOTE: Synthetic Minority Over-sampling Technique).
## Exploratory Data Analysis (EDA)
- Visualized the distribution of NEO features (e.g., miss_distance, relative_velocity) to understand Data Spread.
- Examined data ranges with box plots between features and whether the NEO is hazardous.
- Visualized data density with violin plots between features and target.
- Examined features correlation matrix.
## Feature Extraction
- Using PCA to remove collinearity by transforming the original features into a new set of uncorrelated variables (principal components).
## Modeling Approach
- We evaluated several classification algorithms:
  - Random Forest
  - Logistic Regression
  - KNN
  - XGBoost
  - Gradient Boosting
  - Voting Classifier
  - SVM
## Evaluation Metrics
- We used the following metrics to evaluate model performance:
  - Accuracy: Percentage of correctly predicted NEOs.
  - Precision: Ability to identify hazardous NEOs without misclassifying non-hazardous ones.
  - Recall: Sensitivity to identifying hazardous NEOs.
  - F1-score: Harmonic mean of precision and recall.
  - Learning Curve:  Helps in diagnosing whether your model is overfitting or underfitting.
  - AUC-ROC Curve: Visualize trade-offs between sensitivity and specificity, and provides a single value (AUC) to measure the overall model quality.
## Model Optimization
  - Hyperparameters Tuning using RandomizedSearchCV to avoid model overfitting.
## Results
- The K-Nearest Neighbor (KNN) model achieved the following performance:
  - Accuracy: 95 %
  - Precision: 0.95
  - Recall: 0.94
  - F1-score: 0.94
## Conclusion
- The K-Nearest Neighbor (KNN) model was able to accurately predict hazardous NEOs, making it a reliable model for planetary defense applications. Further tuning and data enrichment could improve the model's predictive power.
## Future Work
- Explore deep learning approaches for enhanced performance.
- Integrate real-time data for continuous model updates.
- Develop a suitable GUI using frameworks that are easy to use.
## References
- NASA's NEO dataset: https://www.kaggle.com/datasets/ivansher/nasa-nearest-earth-objects-1910-2024/data
- Scikit-learn Documentation: https://scikit-learn.org/stable/
- XGBoost Documentation: https://xgboost.readthedocs.io/en/stable/

