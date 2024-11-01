# Machine Learning Project: Regression and Classification

This project uses two separate Jupyter notebooks to perform machine learning on two datasets. One notebook focuses on a **classification** problem, while the other handles a **regression** problem.

---

## Project Structure

- **Classification Notebook**: `classification_weather.ipynb`
    - Dataset: Australian weather data (`weatherAUS.csv`). Available at https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package.
    - Goal: Predict if it will rain tomorrow based on various weather parameters.
    - Models: 
        - K-Nearest Neighbors (KNN)
        - Naive Bayes
        - Neural Network
- **Regression Notebook**: `regression_possum.ipynb`
    - Dataset: Morphometric measurements of possums (`possum.csv`). Available at https://www.kaggle.com/datasets/abrambeyer/openintro-possum.
    - Goal: Predict head length of possums using various physical measurements.
    - Models:
        - Linear Regression
        - Decision Tree
        - Neural Network

---

## Classification Analysis (`classification_weather.ipynb`)

### Data Overview
The classification task uses the `weatherAUS.csv` dataset, containing features related to daily weather conditions in Australia. The target variable is `RainTomorrow`.

1. **Dataset Summary**:
    - Shape and description of data.
    - Check for null values and duplicates.
2. **Exploratory Data Analysis (EDA)**:
    - Frequency distribution of `RainTomorrow`.
    - Visualization of outliers in numerical columns (`Rainfall`, `Evaporation`, `WindSpeed9am`, `WindSpeed3pm`).
    - Data preprocessing with handling missing values, categorical encoding, and scaling.
3. **Modeling**:
    - **K-Nearest Neighbors (KNN)**: Trained on normalized data to predict rainfall.
    - **Naive Bayes**: A probabilistic model applied for binary classification.
    - **Neural Network**: A simple neural network with a binary output for classification.
4. **Results**:
    - Evaluation metrics include accuracy scores for each model.
    - Summary of performance across all models for comparison.

---

## Regression Analysis (`regression_possum.ipynb`)

### Data Overview
The regression task uses the `possum.csv` dataset, containing measurements of different morphometric attributes of mountain possums, aiming to predict head length (`hdlngth`).

1. **Dataset Summary**:
    - Shape, description, and handling of missing values.
2. **Exploratory Data Analysis (EDA)**:
    - Correlation heatmap and distribution plots for numerical columns.
    - Relationship analysis between head length and other features.
3. **Modeling**:
    - **Linear Regression**: A simple regression model to predict head length.
    - **Decision Tree**: A non-linear model used for regression.
    - **Neural Network**: A neural network architecture for regression.
4. **Results**:
    - Evaluation metrics include Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
    - Visual comparisons between actual values and model predictions.