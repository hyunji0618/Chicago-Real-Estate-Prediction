# Chicago Real Estate Price Prediction

## Overview
This project analyzes the **2024 Chicago real estate market** to predict property prices and identify the key factors influencing them. Using a dataset sourced from Kaggle, the project employs robust statistical techniques and feature engineering to develop a high-performing regression model. 

The results offer actionable insights into Chicago's real estate trends and provide a foundation for better decision-making by stakeholders such as buyers, sellers, and investors.

---

## Key Features
- **Baseline and Advanced Models**: 
  - Baseline Ordinary Least Squares (OLS) regression to establish initial benchmarks.
  - Robust Huber Regression for improved accuracy and resilience to outliers.
- **Feature Engineering**:
  - Interaction terms and text-data mapping for deeper insights into property attributes.
  - Forward selection to identify the most impactful features.
- **Model Evaluation**:
  - Comprehensive diagnostics for multicollinearity, heteroskedasticity, and residual normality.
  - Comparison of models based on metrics such as Mean Squared Error (MSE) and \( R^2 \).

---

## Dataset
- **Source**: [Kaggle - Real Estate Data Chicago 2024](https://www.kaggle.com/datasets/kanchana1990/real-estate-data-chicago-2024)
- **Description**: The dataset includes detailed information on property attributes, such as:
  - Property size
  - Number of bedrooms and bathrooms
  - Property type
  - Listed price

---

## Project Highlights
1. **Significant Performance Improvements**:
   - Reduced MSE by **99.99%** and improved \( R^2 \) by **33.18%** using Huber Regression compared to the baseline OLS model.
2. **Key Feature Insights**:
   - Features such as `baths_full` showed the most significant positive impact on property prices.
   - Interaction terms revealed diminishing returns for certain property attributes.
3. **Diagnostic Evaluation**:
   - Addressed multicollinearity and heteroskedasticity using robust statistical methods.

---

## Project Structure
- `final_project.ipynb`: The main Jupyter Notebook containing all analysis, modeling, and evaluation.
- `data/`: Folder for the dataset (not included in this repository; download it from [Kaggle](https://www.kaggle.com/datasets/kanchana1990/real-estate-data-chicago-2024)).
- `outputs/`: Folder containing plots, visualizations, and model outputs.

---

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/chicago-real-estate.git
   cd chicago-real-estate
