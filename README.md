# Predicting Event-Free Survival After Hematopoietic Cell Transplantation (HCT) 

## Project Overview

A passion of mine is to pursue how we can use existing health and social determinants of health data to enhance patient care and improve outcomes. A passion of mine is exploring how existing health and social determinants of health (SDOH) data can be leveraged to enhance patient care and improve outcomes. 

Recently, the Center for International Blood and Marrow Transplant Research (CIBMTR) released a synthetic dataset on [Kaggle](https://www.kaggle.com/competitions/equity-post-HCT-survival-predictions), challenging the machine learning community to develop models that predict event-free survival in hematopoietic cell transplant (HCT) patients. This dataset was synthetically generated from a real CIBMTR cohort using the [SurvivalGAN](https://proceedings.mlr.press/v206/norcliffe23a.html) method. SurvivalGAN captures complex relationships between variables and survival outcomes while sufficiently masking individual data to preserve confidentiality.

A key feature of the dataset is its balanced racial representation, making it ideal for exploring model fairness and performance across different groups. The aim of this project is to predict risk scores using the Stratified Concordance Index (C-index). Features of this metric are:
- Adjusts for racial stratification by calculating the c-index within each racial group
- Rewards models with high accuracy and low variability across groups
- Outputs scores ranging from perfect (1) to worst (0) with 0.5 representing a random prediction.

## Biological Background

HCT is a life-saving treatment used for patients with blood-related cancers and certain immune disorders.  The process involves replacing a patient's disease bone marrow with health stem cells.  

Stem cells can be achieved via two different sources:  Allogeneic or Autologous.  

- An autologous transplant uses patient derived stem cells which are transplanted after a high-dose chemotherapy treatment.  There is a low-risk of immune rejection or graft versus host disease since the patient donates their own stem cells.
- Allogenic transplants utilize stem cells donated by a genetically matched donor.  This type of donation is most appropraite for certain diseases like leukemia and is associated with increased post-transplation event risks from immune complications and graft versus host disease.  The decision of which therapy to use depends on disease type, progression state, patient health and matched donor availability.  

<div align="center"> <img src="https://github.com/user-attachments/assets/959ceff4-0866-4adb-b3e6-f25078e48ed4" alt="Autologous vs Allogeneic Transplant Diagram" width="300"/> </div>


## Project References

Tushar Deshpande, Deniz Akdemir, Walter Reade, Ashley Chow, Maggie Demkin, and Yung-Tsi Bolon. CIBMTR - Equity in post-HCT Survival Predictions. https://kaggle.com/competitions/equity-post-HCT-survival-predictions. Kaggle.
