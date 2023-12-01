# California Housing Price Prediction

 <img src="Elements used/Predicting California Housing Prices with Machine Learning.gif" width="600" height="600" />

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset Description](#dataset-description)
3. [Technical Approach](#technical-approach)
4. [Model Performance Comparison](#model-performance-comparison)
5. [Graphical Representation of Results](#graphical-representation-of-results)
6. [Interpretation of Results](#interpretation-of-results)
7. [How to Run the Project](#how-to-run-the-project)
8. [Engaging Puzzle](#engaging-puzzle)
9. [Conclusion](#conclusion)

## Project Overview
This Python project uses the California Housing dataset to predict housing prices. It demonstrates the application of machine learning techniques including feature selection, dimensionality reduction, and various regression models for accurate price prediction.

## Dataset Description
The dataset encompasses attributes like median income, housing median age, average rooms, average bedrooms, population, occupancy, latitude, and longitude. Each attribute offers a unique perspective on the housing market in California.

## Technical Approach
Our approach includes:
1. **Data Preprocessing**: We standardize features to ensure a consistent scale.
2. **Feature Selection**: Techniques like SelectKBest, RFE, and PCA are used to isolate relevant features.
3. **Model Training and Comparison**: We train Linear Regression, Ridge Regression, Lasso Regression, and Random Forest models, evaluating them for effectiveness.

## Model Performance Comparison
We evaluate model performance based on Mean Squared Error (MSE):

| Model               | MSE with SelectKBest | MSE with RFE | MSE with PCA |
|---------------------|----------------------|--------------|--------------|
| Linear Regression   | 0.6382565            | 0.5667695    | 0.7431025    |
| Ridge Regression    | 0.6382133            | 0.5667326    | 0.7430998    |
| Lasso Regression    | 1.3106960            | 1.3106960    | 1.3106960    |
| Random Forest       | 0.4487779            | 0.2386777    | 0.555144     |

## Graphical Representation of Results
- Visualize MSE values using bar charts for easy comparison.
  
  <img src="Elements used/bar chart gif.gif" width="400" height="400" /><img src="Elements used/bar chart.png" width="400" height="400" />
- Line plots can also be effective in showing model performance over different feature selection methods.
  
  <img src="Elements used/line chart.gif" width="400" height="400" /><img src="Elements used/line chart.png" width="400" height="400" />

## Interpretation of Results


| Model               | MSE (SelectKBest) | MSE (RFE)    | MSE (PCA)    | Interpretation                                             |
|---------------------|-------------------|--------------|--------------|------------------------------------------------------------|
| **Random Forest**   | 0.4487779         | 🏆 0.2386777 | 0.555144     | 🟢 **Best Performance** with RFE, highly accurate.          |
| **Linear Regression** | 0.6382565       | 0.5667695    | 0.7431025    | 🔵 Consistent, slightly higher MSE.                         |
| **Ridge Regression** | 0.6382133       | 0.5667326    | 0.7430998    | 🔵 Similar to Linear, slightly higher MSE.                  |
| **Lasso Regression** | 1.3106960       | 1.3106960    | 1.3106960    | 🔴 Highest MSE, less suitable for this dataset.             |

- 🏆 The **Random Forest** model, especially with RFE, shows the lowest MSE, indicating superior prediction accuracy.
- 🔵 Both **Linear and Ridge Regression** models exhibit similar performances, with slightly higher MSE values than Random Forest.
- 🔴 The **Lasso Regression** model displays the highest MSE, suggesting it's not as effective for this particular dataset.
- These insights help us understand each model's capability in processing and predicting with the dataset's inherent complexity.


## How to Run the Project
- Install Python and necessary libraries (scikit-learn etc.).
- Clone this repository and navigate to the project directory.
- Run `python feature_selection_and_modeling.py`.

## Engaging Puzzle
**Challenge**: Identify a non-intuitive feature that significantly affects housing prices. Explore the dataset and share any surprising findings!

## Conclusion
This project demonstrates real-world application of machine learning in economics, providing valuable insights into housing market analysis.






