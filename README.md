# Multivariate Analysis Project

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Loading Required Packages](#loading-required-packages)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Clustering](#clustering)
- [Principal Component Analysis](#principal-component-analysis)
- [Partial Least Squares Regression](#partial-least-squares-regression)
- [Imputing Missing Values](#imputing-missing-values)
- [Model Comparison](#model-comparison)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction

This project focuses on multivariate analysis of a dataset containing milk sample traits. The primary objectives of the project include:

- Data preprocessing to handle missing values and prepare the dataset for analysis.
- Exploratory Data Analysis (EDA) to gain insights into the dataset and identify patterns.
- Clustering to group observations based on spectral similarity.
- Principal Component Analysis (PCA) to reduce dimensionality and capture essential features.
- Partial Least Squares Regression (PLS) modeling to predict beta lactoglobulin B levels.
- Imputation of missing values using various methods.
- Comparison of different PLS regression models for performance evaluation.

## Getting Started

To run this project locally, follow these steps:

1. Clone this repository.
2. Install the required R packages mentioned in the setup script.
3. Download the dataset (`Milk_MIR_Traits_data_2023.csv`) and place it in the project directory.

## Loading Required Packages

We use several R packages for data analysis and modeling, including:

- `dplyr`
- `tidyverse`
- `ggplot2`
- `ggcorrplot`
- `corrplot`
- `GGally`
- `egg`
- `caret`
- `pls`
- `class`
- `MASS`
- `dendextend`
- `cluster`
- `e1071`
- `mclust`

These packages provide the necessary functions for data manipulation, visualization, clustering, and regression analysis.

## Data Preprocessing

The data preprocessing phase includes the following steps:

- Loading the dataset provided as `Milk_MIR_Traits_data_2023.csv`.
- Removing rows with missing values for `beta_lactoglobulin_b`.
- Handling missing values in the dataset.
- Preparing the dataset for further analysis.

## Exploratory Data Analysis

In this section, we perform detailed exploratory data analysis to gain a deep understanding of the dataset. Key steps include:

- Visualizing protein correlations using correlation plots.
- Analyzing spectral data and plotting MIR spectra.
- Exploring the distribution of `beta_lactoglobulin_b` values.

## Clustering

Two clustering techniques are applied to group observations based on spectral similarity:

1. **Hierarchical Clustering:** The dataset is clustered using complete linkage method, and the results are visualized with a dendrogram.

2. **K-Means Clustering:** The optimal number of clusters is determined using the elbow method, and K-means clustering is performed.

## Principal Component Analysis

Principal Component Analysis (PCA) is employed to reduce dimensionality and capture essential features of the dataset. The optimal number of components is selected using the elbow method, and PCA results are visualized.

## Partial Least Squares Regression

Partial Least Squares Regression (PLS) models are built to predict `beta_lactoglobulin_b` levels. The models are evaluated using cross-validation techniques, and model performance metrics are assessed.

## Imputing Missing Values

Missing values in the `beta_lactoglobulin_b` column are imputed using three different methods:

1. **Data with Non-Zero Values:** Imputing based on records with non-zero values for `beta_lactoglobulin_b`.

2. **Mean Imputation:** Imputing missing values with the mean of non-zero values.

3. **PCA-Based Imputation:** Imputing missing values using PCA on the `beta_lactoglobulin_b` column.

## Model Comparison

The performance of different PLS regression models is compared using RMSE (Root Mean Squared Error) values. Models include:

- Model 1: Using data with non-zero values for `beta_lactoglobulin_b`.
- Model 2: Mean imputation for missing values.
- Model 3: PCA-based imputation for missing values.

## Conclusion

In conclusion, this project provides a comprehensive analysis of multivariate data, including data preprocessing, exploratory analysis, clustering, dimensionality reduction, regression modeling, and missing value imputation. The findings and insights gained from this analysis can be used for further research and decision-making.


## License

This project is licensed under the [MIT License](LICENSE).


## Author 

- **Sarvesh Sairam Naik**

