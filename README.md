
# Residential Electricity Consumption Prediction

## Authors
- Smruthi Bhat
- Aakarsh Bansal

## Abstract
This study aims to develop a data-driven framework for predicting annual household electricity consumption using ensemble learning techniques. The framework involves several stages, including data preprocessing (Exploratory Data Analysis, dimensionality reduction, and feature extraction), identifying relevant features using Information Gain techniques, and applying predictive models. The objective is to provide accurate predictions of household electricity consumption to aid in better resource management and energy conservation.

**Keywords:** Ensemble Learning, EDA, PCA, Dimensionality Reduction

## Table of Contents
- [Introduction](#introduction)
- [Problem Statement and Objectives](#problem-statement-and-objectives)
- [Dataset and Existing Methodology](#dataset-and-existing-methodology)
- [Proposed Approach](#proposed-approach)
- [Experiments and Results](#experiments-and-results)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction
Accurately predicting household electricity consumption is crucial for improving energy efficiency, controlling gas emissions, and optimizing the generation, transmission, and distribution of electrical power. Understanding and predicting residential electricity demand helps residents plan their energy consumption and expenses, fosters energy conservation, and aids in crafting effective energy policies.

## Problem Statement and Objectives

### Problem Statement
To develop a data-driven framework to predict annual household electricity consumption using ensemble learning techniques.

### Objectives
- **Data Pre-Processing:** Utilize techniques like Exploratory Data Analysis (EDA), dimensionality reduction, and feature extraction to enhance data quality and prepare it for modeling.
- **Modeling:** Implement base models such as Extreme Gradient Boosting (XGBoost) and feedforward deep neural networks to capture complex patterns in the data. Experiment with ensemble learning techniques to combine the strengths of multiple models and achieve superior predictive performance.

## Dataset and Existing Methodology

### RECS 2009 Dataset
The RECS 2009 survey collects energy-related data from 12,083 randomly selected households. Despite its extensive coverage, the dataset exhibits a notable presence of missing values, which can impact the analysis and modeling process.

![nonsensical_values](https://github.com/hrtshpdbx/RECS-2009/blob/main/images/nonsense.png) 

### Existing Methodology
- **Feature Selection and Preprocessing:** Reduces the initial 940 attributes to 76 features using subset selection, feature extraction, and PCA.
- **Modeling Approach:** Utilizes ensemble learning to derive insights and predictions but lacks transparency in feature selection and model specifications.

## Proposed Approach

![proposed_approach](https://github.com/hrtshpdbx/RECS-2009/blob/main/images/Proposed_approach.png)

### Exploratory Data Analysis (EDA)
- Conduct comprehensive EDA to gain insights into the dataset's structure and characteristics.
- Identify patterns, distributions, and potential outliers within the data.

### Data Preprocessing
- Handle missing values, outliers, and inconsistencies in the data.
- Employ techniques related to correlation, covariance, and missing value imputation.

![correlation_matrix](https://github.com/hrtshpdbx/RECS-2009/blob/main/images/correlation_matrix.png)

### Feature Scaling, Selection, and Dimensionality Reduction
- Normalize numerical features using Standard Scaling.
- Apply Information Gain and Principal Component Analysis (PCA) for feature selection and dimensionality reduction.

![feature_importance](https://github.com/hrtshpdbx/RECS-2009/blob/main/images/feature_importance.png)

### Modeling
- Develop predictive models using regression algorithms such as linear regression, decision trees, random forests, and gradient boosting.
- Construct an ensemble of models to capture diverse patterns and relationships within the data.
- Fine-tune hyperparameters using Grid Search for optimal performance.

## Experiments and Results
- Conduct extensive data preprocessing, including outlier removal, feature scaling, and dimensionality reduction.
- Implement an ensemble model combining predictions from various base models (Linear Regression, XGBoost, Random Forest, Neural Network).
- Achieve a significant improvement in predictive accuracy, with the ensemble model outperforming individual models and the baseline.

## Conclusion
The proposed data-driven framework leverages ensemble learning techniques and advanced data preprocessing methods to accurately predict annual household electricity consumption. This approach facilitates better resource management, energy conservation, and the development of tailored energy policies.

## References
- Chen, Kunlong, et al. "A novel data-driven approach for residential electricity consumption prediction based on ensemble learning."
- Sagi, Omer, and Lior Rokach. "Ensemble learning: A survey."
- Omuya, Erick Odhiambo, et al. "Feature Selection for Classification using Principal Component Analysis and Information Gain."
- Chen, Tianqi, and Carlos Guestrin. "XGBoost: A scalable tree boosting system."
