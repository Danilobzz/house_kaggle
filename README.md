House Prices Prediction - Kaggle Competition

This project is based on the House Prices: Advanced Regression Techniques competition from Kaggle. The goal is to predict the final price of homes based on various features describing the properties.
Project Overview

This repository contains my approach to building a machine learning model that predicts house prices. The dataset consists of numerous features including house size, location, number of rooms, and various quality indicators. The objective is to build a regression model that can generalize well to unseen data.
Table of Contents

    Data
    Feature Engineering
    Modeling
    Results
    Setup

Data

The dataset is provided by Kaggle and includes the following files:

    train.csv: Contains the training data with target variable SalePrice.
    test.csv: Contains the test data, where SalePrice needs to be predicted.
    
Key Columns:

    Id: Unique identifier for each house.
    SalePrice: The target variable (house price in USD).
    Various categorical and numerical features such as LotArea, YearBuilt, OverallQual, etc.

Feature Engineering

Feature engineering is crucial in improving model performance. The steps performed include:

    Handling Missing Values: Missing values were imputed using strategies like mean, mode, or specific domain knowledge.
    Transforming Categorical Variables: Applied one-hot encoding for categorical variables to allow them to be used in machine learning models.
    Creating New Features: Engineered new features from existing ones (e.g., combining YearBuilt and YearRemodAdd).
    Scaling: Normalized numerical features to ensure consistent scale across different features.

Modeling

The following machine learning models were tested and tuned for optimal performance:

    XGBoost: An optimized gradient boosting algorithm that often performs well in Kaggle competitions.
    Stacking: Combining multiple models to improve prediction accuracy.

The models were evaluated using Root Mean Squared Error (RMSE) on the training data and cross-validated using k-fold cross-validation.
Results

    Best model: XGBoost
    RMSE on validation data: 0.12030710564377811


Acknowledgments

    The dataset is provided by Kaggle.
    The project was made during my Bootcamp in Le Wagon
    Thanks to the open-source community for various tools and libraries such as Pandas, Scikit-learn, XGBoost, and Matplotlib.
