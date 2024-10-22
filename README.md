# Home Loan Default Prediction

This project aims to predict home loan defaults using machine learning techniques, including data cleaning, feature engineering, and classification models. It utilizes models like Random Forest and Neural Networks to classify loan defaults.

## Table of Contents
1. [Project Structure](#project-structure)
   - [1. Data Cleaning and Preparation](#1-data-cleaning-and-preparation)
   - [2. Exploratory Data Analysis (EDA)](#2-exploratory-data-analysis-eda)
   - [3. Feature Engineering](#3-feature-engineering)
   - [4. Modeling](#4-modeling)
2. [Key Findings and Insights](#key-findings-and-insights)
3. [Model Performance](#model-performance)
4. [Suggestions for Improvement](#suggestions-for-improvement)
5. [Conclusion](#conclusion)
6. [Future Work](#future-work)

## Project Structure

### 1. Data Cleaning and Preparation
The project begins by cleaning the dataset, handling missing values, and dropping irrelevant columns.

**Screenshots**:
- Preview of the dataset after cleaning (showing columns retained after handling missing values).

![missingValuesAfter](https://github.com/user-attachments/assets/2075a804-7ec2-46d8-a648-4fc6a63db09d)

- Missing data percentage.

- ![missingValuesBefore](https://github.com/user-attachments/assets/f17e1f44-e884-4374-8cd5-6fa258f76991)

### 2. Exploratory Data Analysis (EDA)
Exploratory analysis of numerical and categorical features is performed to uncover patterns in loan default behavior.

Key Observations:
- Income and credit amounts are highly skewed.
- Default rates are higher among younger individuals and those with shorter employment durations.

**Screenshots**:
- Boxplot for default rates by age group.

![DeafultRatesbyAge](https://github.com/user-attachments/assets/d644a922-0206-4d13-92fd-ae3715cd9a61)

### 3. Feature Engineering
Key features like credit-to-income ratio and aggregated external scores were created to enhance model performance.

### 4. Modeling
Several machine learning models were trained and evaluated, including:
- **Random Forest**: To identify important features.
- **Neural Network**: A deep learning model for classification, tuned using early stopping and model checkpoints.

Key Results:
- Random Forest identified external source scores as the most important features.
- Neural Network achieved high accuracy but required fine-tuning for optimal performance.

**Screenshots**:
- Feature importance plot from Random Forest.

![15importantfeatures](https://github.com/user-attachments/assets/810d9879-cee3-42f0-a703-ee2fe90d61d3)

- Neural network architecture summary (table showing model layers and parameters).

![ModelArchitecture](https://github.com/user-attachments/assets/fcc45fa2-1546-496d-b18c-fef2a2856884)


## Key Findings and Insights
- External source scores (EXT_SOURCE_2, EXT_SOURCE_3) are highly predictive of loan default.
- Younger applicants and those with shorter employment durations have higher default rates.

## Model Performance
- **Random Forest**: Top-performing feature importance model.
- **Neural Network**: Achieved reasonable accuracy with some room for improvement.

## Suggestions for Improvement
1. **Further Tuning**: The Neural Network model can benefit from hyperparameter optimization to reduce overfitting.
2. **Handling Skewed Data**: Investigate outliers in income and credit data to improve model stability.

## Conclusion
The project effectively used machine learning to predict loan defaults, with significant insights gained from external risk scores. However, further refinement of the Neural Network and addressing outliers could improve performance.

## Future Work
1. **Improved Feature Engineering**: Introduce additional external data such as market conditions or economic indicators.
2. **More Robust Modeling**: Explore more advanced neural network architectures like LSTM for time-series elements.
