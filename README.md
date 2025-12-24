# Predicting Drug Overdose Death Rates Using Socioeconomic Indicators

## Overview
This project analyzes the relationship between **socioeconomic factors** and **drug overdose death rates** in the United States and applies **machine learning classification models** to identify patterns associated with higher overdose mortality.

An end-to-end workflow was implemented, including **data integration from multiple public sources**, exploratory data analysis (EDA), feature engineering, and **performance comparison across multiple classification algorithms**.

---

## Problem Statement
Drug overdose deaths remain a major public health crisis in the United States. Understanding how factors such as **unemployment, wages, demographics, and temporal patterns** relate to overdose death rates can help inform policy decisions and prevention strategies.

This project investigates:
- How socioeconomic indicators relate to **drug overdose death rates**
- Whether machine learning models can capture meaningful patterns in overdose mortality
- Which classification models perform best across standard evaluation metrics

---

## Data Sources
Multiple publicly available datasets were integrated for this project.

**Primary Dataset**
- **Drug Overdose Death Rates by Drug Type, Sex, Age, Race, and Hispanic Origin (CDC)**  
  This dataset provides overdose death rates across demographic groups and serves as the primary outcome variable. :contentReference[oaicite:0]{index=0}

**Additional Data Sources**
- Local Area Unemployment Statistics (annual unemployment rate)
- Average Weekly Wages (Quarterly Census of Employment and Wages)
- Provisional drug overdose death counts (death month and drug involvement)

---

## Features Used
Key variables analyzed and engineered include:
- Unemployment Rate (%)
- Average Weekly Wages
- Age Group
- Year
- Death Month
- Demographic encodings (sex, race, Hispanic origin)
- Derived ratios combining socioeconomic and mortality indicators

---

## Exploratory Data Analysis (EDA)
EDA was conducted to understand relationships and distributions:
- Scatter analysis of **unemployment rate vs overdose death rate**
- Correlation matrix to identify feature relationships and multicollinearity
- Distribution analysis across years, demographics, and death months

Key observation:
- Socioeconomic variables show **non-linear and dispersed relationships** with overdose death rates, motivating the use of flexible machine learning models.

---

## Modeling Approach
Although the target variable is **overdose death rates**, the prediction task was framed as a **classification problem** to enable model comparison across multiple performance metrics.

Models evaluated:
- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Gradient Boosting

Each model was trained using the same feature set for a fair comparison.

---

## Model Evaluation
Models were evaluated using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**

### Key Results
- **Gradient Boosting** achieved the strongest overall performance, balancing precision, recall, and F1-score.
- **Random Forest** and **Decision Tree** models showed strong accuracy with moderate trade-offs between recall and precision.
- **KNN** performed poorly in recall, indicating difficulty capturing overdose death patterns.

---

## Visualizations Included
- Unemployment Rate vs Overdose Death Rate scatter plot
- Correlation heatmap of numeric features
- Bar charts comparing models across:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - A project presentation is included as a PowerPoint file.  
  - GitHub does not preview large `.pptx` files — please download to view.

---

## Tools & Libraries
- Python
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- Jupyter Notebook

---

## Repository Structure

predicting-drug-overdose-death-rates/
├── data/
├── notebooks/
├── visuals/
├── results/
├── README.md
└── requirements.txt


