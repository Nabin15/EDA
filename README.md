# Customer Segmentation Exploratory Data Analysis (EDA)

## 📖 Project Overview

This repository contains an **Exploratory Data Analysis (EDA)** for a customer segmentation dataset. The goal of this project is not to build a machine learning model, but to demonstrate comprehensive data exploration and cleaning skills. The analysis involves understanding the structure of the data, handling missing values, and creating insightful visualizations to reveal the underlying distribution of customer attributes and segments.

This EDA serves as the critical first step for any subsequent modeling task, such as building a classifier to segment new potential customers.

## 🧩 Problem Context

An automobile company plans to expand into new markets with its existing products (P1, P2, P3, P4, P5). Based on market research, the new market's customer behavior is expected to be similar to their current market.

In their existing market, the sales team has successfully classified customers into four segments (**A, B, C, D**) and used targeted strategies for each. The company aims to apply this same successful strategy to **2,627 new potential customers** identified in the new markets.

This EDA is performed on the **training dataset** containing the existing customers to understand the patterns that define each segment.

## 📊 Dataset Description

The dataset contains various customer attributes and a target column indicating the segment they belong to.

*   **Source:** https://www.kaggle.com/datasets/vetrirah/customer 
*   **Rows:** The training dataset contains records of existing customers.
*   **Columns:** Features include a mix of demographic and behavioral data (e.g., age, gender, profession, etc.), along with the assigned customer segment.
*   **Target Variable:** `Segment` (A, B, C, D)

## 🛠️ Steps Performed in this EDA

1.  **Data Loading & Initial Inspection:**
    *   Loaded the training dataset.
    *   Checked the first few rows to understand the data structure.
    *   Reviewed data types and basic statistics.

2.  **Data Quality Assessment:**
    *   Identified and quantified **missing values** in each column.
    *   Checked for and removed any **duplicate records**.

3.  **Data Cleaning:**
    *   Handled missing values appropriately based on data type and distribution:
        *   Numerical features: Missing values were replaced with the **median**.
        *   Categorical features: Missing values were replaced with a new category like **'Unknown'** or the **mode**, as suitable.
    *   Ensured the dataset was clean and consistent for analysis.

4.  **Exploratory Data Analysis & Visualization:**
    *   **Univariate Analysis:** Understand the distribution of individual features.
        *   **Histograms** were used for numerical features (e.g., Age, Income).
        *   **Bar charts** and **Pie charts** were used for categorical features (e.g., Gender, Marital Status).
    *   **Target Analysis:** Explored the distribution of the customer `Segment` to check for class balance/imbalance using visualizations.

## 🔮 Conclusion and Next Steps

This EDA provides a solid foundation for understanding the customer base. The data has been thoroughly cleaned and explored, revealing important patterns and relationships.

**Potential Next Steps:**
*   **Feature Engineering:** Create new features from existing ones to improve predictive power.
*   **Model Building:** Train a multi-class classification model (e.g., Random Forest, XGBoost, or a clustering algorithm like K-Means) to predict the segment of new customers.
*   **Model Evaluation:** Validate the model's performance on a hold-out test set.
*   **Deployment:** Deploy the model to classify the 2,627 new potential customers.

## 📝 Dependencies

*   Python 3.x
*   Jupyter Notebook
*   Pandas
*   NumPy
*   Matplotlib
*   Seaborn


---
