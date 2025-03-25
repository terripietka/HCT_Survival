# Predicting Event-Free Survival After Stem Cell Transplantation 

## Project Overview

This project is based on a [Kaggle competition "Equity in post-HCT survival predictions"](https://www.kaggle.com/competitions/equity-post-HCT-survival-predictions) focused on modeling event-free survival for patients who have undergone hematopoietic stem cell transplantation (HSCT). The dataset was synthetically generated using the SurvivalGAN framework, trained on real patient data from the CIBMTR registry.  The data includes 59 demographic and clinical variables for both recipients and donors. 

A key feature of the dataset is its balanced racial representation, making it ideal for exploring model fairness and performance across different groups.  The aim of this project is to predict risk scores using the Stratified Concordance Index (C-index).  Features of this metric are:
- Adjusts for racial stratification by calculating the c-index within each racial group
- Rewards models with high accuracy and low variability across groups
- Outputs scores ranging from perfect (1) to worst (0) with 0.5 representing a random prediction.
