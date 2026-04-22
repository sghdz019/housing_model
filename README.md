# Housing Price Prediction

![R](https://img.shields.io/badge/R-4.0+-blue)
![Model](https://img.shields.io/badge/Model-Regression-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Overview

This project focuses on predicting house prices using machine learning models and feature engineering techniques. The objective is to improve predictive performance by constructing meaningful features and applying robust evaluation methods.

The project includes:

* Data preprocessing and cleaning
* Feature engineering
* Model development and comparison
* Cross-validation for performance evaluation

---

## Methodology

### Feature Engineering

Several features were created to better represent property characteristics, including:

* TotalSF (total square footage)
* TotalBaths
* HouseAge and RemodelAge
* TotalPorchSF
* TotalHomeQuality
* GarageAge
* IsRemodeled
* TotalOutsideSF
* Qual_x_SF (interaction between quality and size)
* Qual_x_Age

These features capture important aspects such as size, quality, and condition of the property.

---

### Model Evaluation

Instead of using a single train/test split, this project applies **5-fold cross-validation** to obtain more stable and reliable performance estimates.

---

## Model Comparison

| Model               | RMSE (CV) |
|--------------------|----------|
| Linear Regression  | ~0.137   |
| Random Forest      | ~0.140   |
| Ridge Regression   | ~0.145   |
| Lasso Regression   | ~0.147   |

Linear Regression achieved the best performance under cross-validation.

---

## Feature Importance

Feature importance was analyzed using the Random Forest model.

The most influential feature is:

* Qual_x_SF (interaction between property quality and size)

This indicates that house prices are strongly influenced by the combined effect of size and quality rather than either factor alone.

---

## Key Insights

* Property size remains a major driver of price
* Construction quality significantly impacts value
* The interaction between size and quality (Qual_x_SF) has the strongest influence
* Feature engineering plays a critical role in improving model performance

---

## Project Structure
