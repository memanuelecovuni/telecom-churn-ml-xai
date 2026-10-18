# Telecommunications Customer Churn Prediction Using Machine Learning and Explainable AI

## Project Overview

This repository contains the Python notebooks developed for an MSc Data Science dissertation at Coventry University.

The project compares five supervised machine learning models (Logistic Regression, Decision Tree, Random Forest, XGBoost and LightGBM) for predicting telecommunications customer churn. It evaluates predictive performance alongside interpretability using intrinsic model characteristics and post-hoc explainability techniques.

## Dataset

The research uses the publicly available *Bulgarian Telecom Business Customer Churn* dataset (Tokmakov, 2024), obtained from Mendeley Data.

The dataset contains 8,453 business customer records, including 549 churn observations (6.49%).

The original dataset is not included in this repository. Users should obtain it from the original data source and configure the relevant file paths before executing the notebooks.

## Repository Structure

The notebooks are organised in execution order:

1. **01_Data_Preparation_EDA_and_Feature_Engineering.ipynb** — Data loading, exploratory data analysis, feature engineering, preprocessing and preparation of modelling datasets.
2. **02_Model_Development_and_Evaluation.ipynb** — Model training, class-imbalance treatment, hyperparameter optimisation and predictive-performance evaluation.
3. **03_Model_Explainability_and_Final_Assessment.ipynb** — Model interpretation, SHAP analysis, perturbation analysis and final model comparison.
4. **04_Tableau_Data_Export_and_Dashboard_Preparation.ipynb** — Preparation and export of data sources used to construct the Tableau dashboards.

## Software and Execution

The notebooks were developed using Python in Google Colab, with Google Drive used for file storage.

Key libraries include PySpark, pandas, NumPy, scikit-learn, XGBoost, LightGBM, SHAP, Matplotlib and SciPy.

To reproduce the workflow:

1. Obtain the original dataset from its published source.
2. Configure the dataset, Google Drive and output paths within the notebooks.
3. Install the required Python libraries and compatible dependencies.
4. Execute the notebooks sequentially, from 01 to 04.
5. Retain the intermediate datasets and model artefacts required by subsequent notebooks.

Some stages require substantial processing resources, and results may depend on library versions and execution environment.

## Evaluation and Explainability

Predictive performance is evaluated using accuracy, precision, recall, F1-score, ROC-AUC and PR-AUC, with particular attention to identifying the minority churn class.

Explainability includes Logistic Regression coefficients, Decision Tree structure, SHAP-based feature attribution and perturbation analysis. Global explanations are compared across nonlinear models, with additional local explanations for the selected model.

The study assesses predictive associations and model behaviour; the explanations do not establish causal relationships.

## Research Scope

The repository supports the dissertation's experimental analysis and Tableau data preparation. It does not provide a deployed prediction system or demonstrate the effectiveness of customer retention interventions.

## Submission Record

This repository forms part of the MSc dissertation artefact submitted to Coventry University. The submitted repository version will be preserved without changes for at least three months following dissertation submission.
