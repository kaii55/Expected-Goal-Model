# Expected-Goal-Model

Chance Quality Models for Football Shots

# Overview

This repository contains models and data analyses related to the prediction of goal probabilities for football shots using advanced machine learning techniques. The main objective of this project is to measure the quality of a shot by calculating the probability of it resulting in a goal. This analysis is based on event and tracking data provided by Metrica Sports, with models developed and evaluated on various datasets.

# Contents

Task 1: Chance Quality Model for Football Shots
Objective: Measure the quality of a chance by calculating the probability of a shot resulting in a goal.
Methodology:
Data pre-processing and feature engineering (coordinate conversion to OPTA format, feature selection, and creation).
Model selection: Logistic Regression, XGBoost, and Artificial Neural Networks (ANN).
Evaluation: Models evaluated using RMSE, Brier Score, AUC, and confusion matrix metrics.
Visualization: Results and predictions visualized using PCA and t-SNE to illustrate model effectiveness in low-dimensional space.
Notebooks:
Task 1 - xG (Shot and Goal Viz.).ipynb: Visualization and initial modeling.
Task 1 - xG - (XGBoost) [Cross-Validation].ipynb: Cross-validation analysis of XGBoost.
Task 1 - xG - (ANN) [Cross-Validation].ipynb: Cross-validation analysis of ANN.
Task 2: Shooting Opportunities and Advanced Metrics
Objective: Extend the chance quality model to predict the expected goals (xG) from different zones on the pitch and under various conditions (open play, set-pieces).
Methodology:
Data integration and pre-processing (event and tracking data from Metrica Sports Match-2).
Advanced features: Player positioning, interference calculations, shot distance and angle measurements, and pitch zone assignments.
Model application: XGBoost and cost-sensitive ANN models used to predict scoring probabilities.
Evaluation: Compare xG predictions with actual outcomes using detailed metrics for open play and set-piece situations.
Notebooks:
Task 2 - xG - (XGBoost) + metrica.ipynb: Detailed results using XGBoost.
Task 2 - xG - (ANN) + metrica.ipynb: Detailed results using ANN.

# Key Features

Data Engineering: Processing and integration of event and tracking data with coordinate transformation and feature extraction.
Modeling: Comparison of Logistic Regression, XGBoost, and ANN models to predict scoring chances. Evaluation through metrics such as RMSE, Brier Score, AUC, and detailed confusion matrices.
Feature Importance: Analysis of the significance of various features (e.g., shot angle, number of intervening opponents, body part used) on the scoring probability.
Visualization: Use of PCA and t-SNE for data visualization, alongside detailed shot visualizations on a football pitch to illustrate model predictions.
Expected Goals from Set Plays: Includes the analysis of expected goals from corners, free kicks, and penalties, with a focus on how these set-piece opportunities contribute to overall scoring chances.
