# Ames Housing - EDA & Data Preprocessing Pipeline 🏡

## Project Overview

This is an educational data science project focused on **Exploratory Data Analysis (EDA)**, **feature engineering**, and building robust **data preprocessing pipelines**. The project uses the famous Ames Housing dataset.

## Key Learnings & Techniques Applied

- **Exploratory Data Analysis (EDA):** Visualized numerical and categorical features using `seaborn` and `pandas` to understand distributions and relationships with house prices.
- **Handling Structural Missingness:** Investigated the difference between Missing Completely at Random (MCAR) and Missing Not at Random (MNAR), specifically how `NaN` in Ames Housing often means the physical absence of a feature (e.g., "No Garage").
- **Feature Engineering:** Created and validated new features like `Has_Garage` logically against existing area metrics.
- **Robust Scikit-Learn Pipelines:** Built clean `Pipeline` and `ColumnTransformer` workflows to separate numerical (Scaling/Median Imputation) and categorical (OHE/Imputation) data.
- **Preventing Data Leakage:** Ensured strict `fit_transform` on training data and `transform` on testing data, alongside utilizing `handle_unknown="ignore"` for production-safe One-Hot Encoding.

## Technologies Used

- Python 3
- Pandas & NumPy
- Seaborn & Matplotlib
- Scikit-Learn
