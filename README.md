# Advanced-Programming-UC3M
# Predicting Wind Energy Production with Scikit-Learn

## Introduction

The forecasting of energy generation 24 hours in advance is essential for planning energy plants' operations to meet the next day's supply and demand. Unlike traditional energy sources, solar and wind energies depend on weather conditions and thus require accurate forecasting. This project utilizes meteorological variables forecasted by the ECMWF to estimate the energy produced at the Sotavento experimental wind farm through machine learning models.

## Project Overview

The goal of this project is to employ machine learning techniques to predict wind energy production accurately. We take in meteorological forecast data as input attributes to model the electricity generation at Sotavento, an experimental wind farm. Due to the indirect relationship between weather variables and actual electricity production, this project explores the efficacy of machine learning models in closing this gap.

## Dataset

The data includes 22 meteorological variables from the ECMWF, instantiated across a 5x5 grid surrounding the Sotavento location, resulting in 550 input attributes per instance. Variables range from those directly related to wind energy, like the "100 metre U wind component", to less apparent ones, such as "Leaf area index high vegetation".

## Methodology

1. **Data Exploration and EDA**: Initial data exploration to identify features, instances, and handle missing values.
2. **Data Splitting**: Considering the data's nature (i.i.d. vs. non-i.i.d.), the dataset was split into training and testing sets.
3. **Model Evaluation**: Initial evaluation was performed using Trees and KNN with default hyper-parameters. For KNN, preprocessing (scaling) was included in the pipeline.
4. **Hyper-parameter Tuning (HPO)**: Trees and KNN models underwent HPO to optimize performance.
5. **Feature Selection**: Utilizing SelectKBest with criteria like f_classif and mutual_info_classif to identify the most relevant features for KNN.
6. **Model Finalization and Prediction**: The best-performing model was used to estimate errors and make predictions on the competition dataset.

## Tools and Technologies

- Python
- Scikit-Learn for machine learning models
- Google Colab for analysis and documentation

## How to Use

The repository contains a pynb file detailing the analysis process, from data exploration to final model predictions.

## Collaboration

This project was developed with Marcos Crespo as part of [MSc Statistics for Data Science/UC3M],


