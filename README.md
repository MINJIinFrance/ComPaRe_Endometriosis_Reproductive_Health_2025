 # ComPaRe Endometriosis: Reproductive Health Analysis

This repository contains the data management and statistical analysis pipeline for my **Master’s Thesis** conducted at the **Center for Research in Epidemiology and Population Health (CESP)** - Inserm U1018, in collaboration with Institut Gustave Roussy.

## 📌 Project Overview
The study investigates the reproductive journey and pregnancy outcomes of women with endometriosis using data from the **ComPaRe-Endometriosis e-cohort** (Communauté de Patients pour la Recherche).

### Research Objectives
1. **Descriptive Analysis**: Comprehensive overview of reproductive health in women with endometriosis.
2. **Factors Associated with Live Births**: Identifying sociodemographic and clinical predictors of successful live births.
3. **Obstetrical Complications**: Analyzing risk factors associated with pregnancy-related complications (e.g., Preeclampsia, Gestational Diabetes, Preterm birth).

## 🛠 Tech Stack & Methodology
* **Language:** R (v4.3.3)
* **Data Management:** * Cleaning and merging complex longitudinal data from multiple patient-reported questionnaires (PROMs).
    * Handling missing data using **missForest** (Random Forest-based imputation).
* **Statistical Modeling:**
    * **Binary Logistic Regression**: For live birth and general complication factors.
    * **Multinomial Logistic Regression**: For categorized obstetrical complication types.
    * **Validation**: Multicollinearity assessment via Variance Inflation Factor (VIF).

## 📂 Repository Structure
```text
├── Data_Cleaning/           # Scripts for cleaning 10+ survey modules
├── Data_Merge/              # Logic for merging inclusion & pregnancy datasets
├── EDA/                     # Exploratory analysis & data visualization
└── Statistical_Analysis/    # Final regression models (Logit/Multinominal)
