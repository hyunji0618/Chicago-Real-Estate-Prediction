# Chicago Real Estate Price Prediction

## Overview
This project analyzes the **2024 Chicago real estate data** to predict property prices and identify the key factors influencing them. Using a dataset sourced from Kaggle, the project employs robust statistical techniques and feature engineering to develop a high-performing regression model. 

The results aim to offer actionable insights into Chicago's real estate trends and provide a foundation for better decision-making by stakeholders such as buyers, sellers, and investors.

---

## Key Features
- **Baseline and Advanced Models**: 
  - Baseline Ordinary Least Squares (OLS) regression to establish initial benchmarks.
  - Robust linear regression models like Lasso and Ridge Regression.
  - Robust Huber Regression for improved accuracy and resilience to outliers.
- **Feature Engineering**:
  - Interaction terms and text-data mapping for deeper insights into property attributes and their impact on the dependent variable (Price).
  - Forward selection to identify the most impactful features.
- **Model Evaluation**:
  - Comprehensive diagnostics such as multicollinearity, heteroskedasticity, and residual normality.
  - Comparison of models based on metrics such as Mean Squared Error (MSE) and \( R^2 \) scores.

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
   - Improved \( R^2 \) by **33.18%** and reduced MSE by **99.99%** and using Huber Regression compared to the baseline OLS model.
2. **Key Feature Insights**:
   - Features such as `baths_full` showed the most significant positive impact on property prices.
   - Interaction terms revealed diminishing returns for certain property attributes.
3. **Diagnostic Evaluation**:
   - Addressed multicollinearity and heteroskedasticity using robust statistical methods.

---

## Project Structure
- `real_estate_prediction_model.ipynb`: The main Jupyter Notebook containing all analysis, modeling, and evaluations, along with comprehensive explanations.
- `real_estate_data_chicago.csv`: CSV file for the dataset (can also be downloaded from [Kaggle](https://www.kaggle.com/datasets/kanchana1990/real-estate-data-chicago-2024)).

---

## Results

The performance of the models was evaluated based on various metrics, including Mean Squared Error (MSE), Mean Absolute Error (MAE), \(R^2\), and Adjusted \(R^2\). The results demonstrate significant improvements achieved through robust regression techniques and feature engineering.

### Baseline OLS Regression (No Preprocessing)
- **\(R^2\)**: 0.5618
- **Adjusted \(R^2\)**: 0.5477
- **MSE**: 623,761,136,340.02
- **MAE**: 380,299.01

### Final Huber Regression Model
- **\(R^2\)**: 0.7478 (Improved by **33.18%** from OLS)
- **Adjusted \(R^2\)**: 0.7264 (Improved by **32.71%** from OLS)
- **MSE**: 0.2631 (Reduced by **99.99%** compared to OLS)
- **MAE**: 0.3928 (Reduced by **99.90%** compared to OLS)

The Huber Regression model significantly outperformed the baseline. This result effectively demonstrates its robustness in handling outliers and heavy-tailed residuals, and highlights the importance of advanced preprocessing and robust regression techniques.

---

## Future Works

While the project achieved substantial improvements, there are several opportunities for further exploration:

1. **Addressing Heavy-Tailed Residuals**  
   - Implement a **GAMLSS model** with a t-distribution to better capture heavy-tailed behavior in residuals.

2. **Exploring Non-Linear Relationships**  
   - Investigate more complex non-linear interactions between features beyond log transformations and second-order interactions.

3. **Advanced Modeling Techniques**  
   - Apply machine learning methods such as Random Forests, Gradient Boosting, or Neural Networks to explore non-linear dependencies.
     
4. **Enhanced Feature Engineering**
   - Incorporate external datasets, such as neighborhood crime rates, school ratings, or proximity to amenities, to improve the explanatory power of the model. Explore advanced feature selection techniques to refine the input variables further.
   
