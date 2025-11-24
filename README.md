Clustering and Fitting Analysis of Global CO2 Emissions

Author: QUMRISH AROOJ

Overview

This repository contains the code and outputs for a Clustering and Fitting analysis performed on global CO2 emissions data. The project demonstrates how to explore and model country-level CO2 per capita patterns using statistical summaries, K-Means clustering, and regression techniques.

The assignment includes data cleaning, descriptive statistics, visualization, clustering, regression modeling, and report generation.

Dataset

The analysis uses the OWID CO2 Dataset (1990–2019), which contains country-level information on:

CO2 emissions (co2, co2_per_capita)

Consumption-based CO2 (consumption_co2)

Population and GDP

Greenhouse gas indicators (total_ghg, ghg_per_capita)

Energy consumption indicators (primary_energy_consumption, energy_per_capita, energy_per_gdp)

Note: Aggregate rows such as OWID regions were removed to focus on individual countries.

Repository Structure
clustering_fitting_assignment/
│
├─ outputs/                     # Generated plots and CSV files
│   ├─ categorical_top10_co2_2019.png
│   ├─ relational_gdp_vs_co2_2019.png
│   ├─ heatmap_2019.png
│   ├─ boxplot_co2_by_gdp_decile_2019.png
│   ├─ kmeans_elbow.png
│   ├─ kmeans_k*_pca.png
│   ├─ pairplot_moments.png
│   ├─ regression_actual_vs_predicted_ridge.png
│   ├─ country_moments.csv
│   └─ descriptive_co2_per_capita.txt
│
├─ clustering_fitting_assignment.py  # Main Python script
├─ README.md                        # This file
└─ assessment.txt                   # Short assessment summary

Requirements

The code was developed using Python 3.11 and the following libraries:

numpy

pandas

matplotlib

seaborn

scipy

scikit-learn

You can install the dependencies using pip:

pip install numpy pandas matplotlib seaborn scipy scikit-learn

Usage

Clone the repository:

git clone https://github.com/your-username/clustering_fitting_assignment.git
cd clustering_fitting_assignment


Place the OWID CO2 dataset CSV (owid-co2-data.csv) in the repository folder.

Run the Python script:

python clustering_fitting_assignment.py


All outputs (plots, CSVs, metrics) will be saved in the outputs/ folder.

Analysis Highlights

Descriptive Statistics: Computed country-level moments of CO2 per capita, including mean, standard deviation, skewness, and kurtosis.

Visualization:

Bar chart of top 10 CO2 emitting countries

Scatter plot of CO2 per capita vs GDP

Heatmap of correlations

Boxplot of CO2 per capita by GDP deciles

Clustering:

K-Means clustering on country-level CO2 patterns

Elbow and silhouette analysis to select the optimal number of clusters

PCA projection to visualize clusters

Regression (Fitting):

Linear and Ridge regression to predict CO2 per capita using log-transformed GDP and population

Performance metrics: R², RMSE, MAE

Outputs: All plots and metrics are saved in the outputs/ folder.

Files in Outputs

country_moments.csv — Per-country CO2 per capita moments

categorical_top10_co2_2019.png — Top 10 countries by CO2

relational_gdp_vs_co2_2019.png — CO2 per capita vs GDP

heatmap_2019.png — Correlation heatmap

boxplot_co2_by_gdp_decile_2019.png — CO2 per capita by GDP decile

kmeans_elbow.png — Elbow plot for clustering

kmeans_k*_pca.png — PCA visualization of clusters

pairplot_moments.png — Pairplot of CO2 per capita moments

regression_actual_vs_predicted_ridge.png — Actual vs predicted CO2 per capita

descriptive_co2_per_capita.txt — Summary statistics
