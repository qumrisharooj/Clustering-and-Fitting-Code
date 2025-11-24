# Clustering and Fitting Analysis of Global CO2 Emissions

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![License](https://img.shields.io/badge/License-Educational-lightgrey)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

**Author:** QUMRISH AROOJ
---

## Overview

This project demonstrates a **comprehensive analysis of global CO2 emissions per capita** across countries using **statistical analysis, clustering (K-Means), and regression techniques**.  

The main goals are:  

- Explore and visualize CO2 emission trends.  
- Cluster countries based on CO2 per capita patterns.  
- Predict CO2 per capita using GDP and population.  
- Generate professional plots and CSV outputs for reporting.  

**Dataset:** [OWID CO2 Dataset (1990–2019)](https://ourworldindata.org/co2-and-other-greenhouse-gas-emissions)  

---

## Table of Contents

1. [Project Features](#project-features)  
2. [Repository Structure](#repository-structure)  
3. [Getting Started](#getting-started)  
4. [Usage](#usage)  
5. [Outputs](#outputs)  
6. [Insights](#insights)  
7. [License](#license)  

---

## Project Features

- **Data Cleaning & Preparation**  
  - Filtered data from 1990–2019  
  - Removed OWID region aggregates  
  - Dropped missing values in key columns  

- **Statistical Analysis**  
  - Calculated per-country moments: mean, std, skewness, kurtosis  
  - Descriptive summary of CO2 per capita  

- **Visualizations**  
  1. Bar chart: Top 10 CO2 emitting countries  
  2. Scatter plot: CO2 per capita vs GDP  
  3. Heatmap: Correlation among numeric features  
  4. Boxplot: CO2 per capita by GDP deciles  

- **Clustering (K-Means)**  
  - Features: mean CO2 per capita, std CO2 per capita, optional mean GDP  
  - Optimal number of clusters selected using silhouette score and elbow method  
  - PCA projection used for 2D visualization of clusters  

- **Regression Analysis**  
  - Linear Regression and Ridge Regression  
  - Features: log-transformed GDP and log-transformed population  
  - Evaluation metrics: RMSE, MAE, R²  

---

## Repository Structure

clustering_fitting_assignment/
│

├─ clustering_fitting_assignment.py # Main Python script

├─ outputs/ # Generated plots and CSVs

│ ├─ categorical_top10_co2_2019.png

│ ├─ relational_gdp_vs_co2_2019.png

│ ├─ heatmap_2019.png

│ ├─ boxplot_co2_by_gdp_decile_2019.png

│ ├─ kmeans_elbow.png

│ ├─ kmeans_k*_pca.png

│ ├─ pairplot_moments.png

│ ├─ regression_actual_vs_predicted_ridge.png

│ ├─ country_moments.csv

│ └─ descriptive_co2_per_capita.txt

├─ assessment.txt # Short assessment summary

└─ README.md # Project documentation



## Getting Started

### Prerequisites

- Python 3.7+  
- Required libraries:  

```bash
pip install numpy pandas matplotlib seaborn scipy scikit-learn


python clustering_fitting_assignment.py


