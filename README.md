# Nearest-Earth-Objects-Prediction
## Project Overview
In this project, we analyze a real-world dataset tracking 338,199 Near-Earth Objects (NEOs) observed by NASA between 1910 and 2024. The goal is to develop a machine learning model that can accurately predict whether a NEO poses a potential hazard to Earth, as indicated by the "is_hazardous" classification. Accurately identifying dangerous NEOs is crucial for planetary defense and ensuring preparedness for potential threats. The project will involve data preprocessing, feature selection, and model training to classify NEOs based on their proximity and characteristics.
## Dataset
Dataset contains many features includes:
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
## Exploratory Data Analysis (EDA)
- Visualized the distribution of NEO features (e.g., miss_distance, relative_velocity) to understand Data Spread.
- Examined data ranges with box plots between features and whether the NEO is hazardous.
- Visualized data density with violin plots between features and target.
- Examined features correlation matrix.
