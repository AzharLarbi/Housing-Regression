# Housing Prices Regression

This project uses a regression model to predict housing prices based on a range of property characteristics, including both numerical and categorical features. The aim is to analyze how each feature impacts housing prices and to develop a predictive model with effective accuracy.

# Project Overview

The project explores how various features of a property impact its price, using a regression model that incorporates both numerical and categorical variables. After encoding categorical features, a linear regression model was trained to predict housing prices. While additional features were added, the initial model's loss did not improve significantly, indicating potential areas for further tuning and experimentation.

# Objectives

Visualize and understand the relationships between different features and housing prices.

Build a regression model that uses all available features to improve predictions.
Explore further improvements through advanced modeling and tuning techniques.

# Dataset

The dataset used is House Price Prediction Dataset.csv, which can be downloaded from kaggle: https://www.kaggle.com/datasets/zafarali27/house-price-prediction-dataset/data
It containing 2,000 entries with the following attributes:

Area: Total area of the house.

Bedrooms: Number of bedrooms.

Bathrooms: Number of bathrooms.

Floors: Number of floors in the house.

YearBuilt: The year the house was constructed.

Location: General location category of the property.

Condition: Property condition (e.g., new, good).

Garage: Garage availability.

Price: Target variable representing the house price.

# Exploratory Data Analysis

The notebook includes detailed data visualizations for key features:

Distributions of features like Area, Bedrooms, Bathrooms, and YearBuilt.

Target Variable Distribution: Price distributions are analyzed across categorical features such as Garage, Location, and Condition.

Correlation Heatmap: A heatmap is used to examine correlations among numerical features, identifying features that have a stronger association with Price.

# Modeling

The project utilizes the following steps for modeling:

Feature Selection and Encoding: All features are included, with categorical features encoded for use in the model.

Model Training: A linear regression model from scikit-learn is trained using both numerical and encoded categorical features.

Evaluation: Performance is measured with RMSE (Root Mean Squared Error) using a custom function:
```
def rmse(targets, predictions):
    return np.sqrt(np.mean(np.square(targets - predictions)))
```
# Usage

To use this project:

Data Preprocessing and EDA: Run the cells in the notebook to load, clean, encode, and explore the data.

Model Training and Evaluation: Train the model using all features and evaluate its performance.

# Results

After training with all available features, the model’s RMSE was around (insert RMSE from results), with limited improvement observed from categorical encoding.

# Contributing

Contributions are welcome! Potential areas for improvement include:

Hyperparameter tuning to enhance model performance.

Trying alternative models, such as decision trees or ensemble methods.

Performing feature selection or dimensionality reduction to analyze feature impact.
    
