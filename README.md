# Predicting Event-Free Survival After Hematopoietic Cell Transplantation (HCT) 

## Project Overview

A passion of mine is to pursue how we can use existing health and social determinants of health data to enhance patient care and improve outcomes. A passion of mine is exploring how existing health and social determinants of health (SDOH) data can be leveraged to enhance patient care and improve outcomes. 

Recently, the Center for International Blood and Marrow Transplant Research (CIBMTR) released a synthetic dataset on [Kaggle](https://www.kaggle.com/competitions/equity-post-HCT-survival-predictions), challenging the machine learning community to develop models that predict event-free survival in hematopoietic cell transplant (HCT) patients. This dataset was synthetically generated from a real CIBMTR cohort using the [SurvivalGAN](https://proceedings.mlr.press/v206/norcliffe23a.html) method. SurvivalGAN captures complex relationships between variables and survival outcomes while sufficiently masking individual data to preserve confidentiality.

A key feature of the dataset is its balanced racial representation, making it ideal for exploring model fairness and performance across different groups. The aim of this project is to predict risk scores using the Stratified Concordance Index (C-index). Features of this metric are:
- Adjusts for racial stratification by calculating the c-index within each racial group
- Rewards models with high accuracy and low variability across groups
- Outputs scores ranging from perfect (1) to worst (0) with 0.5 representing a random prediction.
