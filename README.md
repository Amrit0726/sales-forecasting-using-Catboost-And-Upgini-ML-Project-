# Sales Forecasting using CatBoost and Upgini

## Introduction
This project is part of my learning journey in **Machine Learning and Time Series Analysis**.
The goal of the project is to build a regression model that can predict sales values
using historical time-based data and to understand how **feature engineering** can
improve model performance.

---

## Problem Statement
Given time-indexed sales data, the task is to predict future sales values.
Since the data is time-dependent, special care is taken to avoid data leakage
while splitting and evaluating the model.

---

## Approach
1. Performed basic data understanding and preprocessing  
2. Built a baseline **CatBoost Regressor** model  
3. Evaluated the model using **SMAPE / MAPE** metrics  
4. Experimented with **external feature enrichment** using Upgini  
5. Compared baseline and enriched model performance  

---

## Feature Enrichment Experiment
To explore how external data can help improve predictions, I used the **Upgini**
feature enrichment platform, which generates additional temporal and contextual features.

Due to trial API limitations, enrichment was demonstrated on a limited subset of the data.
Even with this constraint, the enriched features showed a noticeable reduction in prediction
error compared to the baseline model.

---

## Results (Summary)
- Baseline model trained using original features  
- Enriched model trained with additional external features  
- Error reduced by approximately **21–24%** on evaluation data after enrichment  

These results indicate that external features can add useful information for
time-series forecasting problems.

---

## What I Learned
- How to handle time-series data in regression problems  
- Using CatBoost for regression tasks  
- Importance of evaluation metrics like SMAPE and MAPE  
- Practical challenges of using third-party APIs in ML projects  
- How feature engineering can significantly impact model performance  

---

## Tools & Libraries
- Python  
- Pandas, NumPy  
- CatBoost  
- Upgini  

---

## Notes
- API keys are not included in this repository for security reasons  
- Results may vary due to sampling, randomness, and external API constraints  

---

## Author
Amrit Noor Singh
