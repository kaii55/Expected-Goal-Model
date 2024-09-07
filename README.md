# Chance Quality Models for Football Shots

## Overview

This repository contains models and data analyses focused on predicting the goal probabilities of football shots using advanced machine learning techniques. The primary goal of this project is to measure the quality of a shot by calculating the probability of it resulting in a goal. The analysis is based on event and tracking data provided by Metrica Sports, with models developed and evaluated on various datasets. 

Please refer to the ##1. ChanceQualityModel.pptx ##2. ShootingOpportunities.pptx for an in-detail overview.

## Contents

### Task 1: Chance Quality Model for Football Shots

- **Objective:** Measure the quality of a chance by calculating the probability of a shot resulting in a goal.
- **Methodology:**
  - **Data Pre-processing and Feature Engineering:** Converting coordinates to OPTA format, feature selection, and creation.
  - **Model Selection:** Using Logistic Regression, XGBoost, and Artificial Neural Networks (ANN) to build predictive models.
  - **Evaluation Metrics:** Models are evaluated using metrics such as RMSE, Brier Score, AUC, and confusion matrices.
  - **Visualization:** Data is visualized using PCA and t-SNE, illustrating model effectiveness in low-dimensional space.
- **Notebooks:**
  - `Task 1 - xG (Shot and Goal Viz.).ipynb`: Visualization and initial modeling.
  - `Task 1 - xG - (XGBoost) [Cross-Validation].ipynb`: Cross-validation analysis of XGBoost.
  - `Task 1 - xG - (ANN) [Cross-Validation].ipynb`: Cross-validation analysis of ANN.

### Task 2: Shooting Opportunities and Advanced Metrics

- **Objective:** Extend the chance quality model to predict expected goals (xG) from various zones on the pitch and under different conditions (open play, set-pieces).
- **Methodology:**
  - **Data Integration and Pre-processing:** Processing event and tracking data from Metrica Sports Match-2.
  - **Advanced Features:** Analyzing player positioning, calculating interference, shot distances, shot angles, and pitch zone assignments.
  - **Model Application:** Applying XGBoost and cost-sensitive ANN models to predict scoring probabilities.
  - **Evaluation:** Comparing xG predictions with actual outcomes using detailed metrics for open play and set-piece situations.
- **Notebooks:**
  - `Task 2 - xG - (XGBoost) + metrica.ipynb`: Detailed results using XGBoost.
  - `Task 2 - xG - (ANN) + metrica.ipynb`: Detailed results using ANN.

## Key Features

- **Data Engineering:** Processing and integrating event and tracking data with coordinate transformation and feature extraction.
- **Modeling:** Comparing Logistic Regression, XGBoost, and ANN models to predict scoring chances, evaluated through RMSE, Brier Score, AUC, and confusion matrices.
- **Feature Importance:** Analysis of key features (e.g., shot angle, number of intervening opponents, body part used) affecting scoring probabilities.
- **Visualization:** Utilizing PCA and t-SNE for data visualization, alongside detailed shot visualizations on a football pitch.
- **Expected Goals from Set Plays:** Includes analyses of expected goals from corners, free kicks, and penalties, highlighting the impact of set-piece opportunities.

## Results

### Task 1: Chance Quality Model

- **Models Evaluated:**
  - Logistic Regression, XGBoost, and ANN.
- **Performance Metrics:**
  - **Logistic Regression:**
    - RMSE: 0.2877, AUC: 0.60, Brier Score: 0.082.
  - **XGBoost:**
    - RMSE: 0.2865, AUC: 0.60, Brier Score: 0.081.
  - **ANN:**
    - RMSE: 0.2882, AUC: 0.60, Brier Score: 0.083.
- **Key Findings:**
  - Cost-sensitive models show better performance with lower RMSE and Brier scores.
  - Important features include shot angle, number of intervening opponents, and the body part used.

### Task 2: Shooting Opportunities and Advanced Metrics

- **Expected Goals Predictions:**
  - **XGBoost:** xG predicted for Home Team: 2.10, Away Team: 2.41.
  - **ANN Cost-Sensitive:** xG predicted for Home Team: 1.87, Away Team: 1.98.
- **Set Piece Analysis:**
  - Set-piece xG calculated for corners, free kicks, and penalties with specific metrics highlighting team proficiency in dead-ball situations.
- **Model Performance:**
  - Models show variability in accuracy across different zones, with some overestimations and underestimations identified.
  - Zone-specific analysis reveals areas of high scoring accuracy and those requiring model improvement.

