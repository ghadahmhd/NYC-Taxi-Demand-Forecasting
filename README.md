# Big Data Analysis and Forecasting of NYC Taxi Demand Using Machine Learning Techniques

## Overview

This project presents a Big Data analytics and machine learning framework for analyzing and forecasting New York City taxi demand using NYC Yellow Taxi trip records.

The project combines distributed data processing, unsupervised learning, supervised classification, and time-series forecasting to identify transportation patterns and predict taxi demand.

## Objectives

- Analyze large-scale NYC taxi trip data.
- Identify trip behavior patterns using K-Means clustering.
- Classify taxi demand into low, medium, and high levels using Decision Tree classification.
- Forecast future taxi demand using ARIMA.
- Evaluate model performance using appropriate evaluation metrics.

## Dataset

**Source:** NYC Taxi and Limousine Commission (TLC)

**Dataset:** Yellow Taxi Trip Records

**Time Period:** January 2025 – May 2025

**Dataset size:**
- Initial dataset: More than 7 million records.
- After preprocessing: More than 5.4 million records.

**Main features:**
- Pickup and drop-off timestamps
- Passenger count
- Trip distance
- Fare amount
- Pickup and drop-off locations

Official dataset: https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

## Technologies and Tools

- Python
- PySpark
- Apache Spark
- Pandas
- Matplotlib
- Scikit-learn
- Statsmodels
- Google Colab

## Methodology

The project consists of four main stages:

### 1. Data Preprocessing
- Handling missing values.
- Removing invalid records.
- Filtering extreme outliers.
- Feature engineering.
- Extracting time-related features.

### 2. K-Means Clustering
K-Means was used to discover patterns in taxi trip behavior.

- Cluster selection: Elbow Method.
- Selected clusters: K = 4.
- Evaluation: Silhouette Score.

### 3. Decision Tree Classification
A Decision Tree classifier was developed to predict taxi demand levels.

Demand categories:
- Low Demand
- Medium Demand
- High Demand

The model was evaluated using a train-test split and classification accuracy.

### 4. ARIMA Forecasting
ARIMA was applied to historical daily taxi trip counts to forecast future demand.

The forecasting model was evaluated using Root Mean Squared Error (RMSE).

## Experimental Results

| Model | Evaluation Metric | Result |
|---|---|---:|
| K-Means | Silhouette Score | 0.804 |
| Decision Tree | Test Accuracy | 61.9% |
| ARIMA | Test RMSE | 20,433.77 |

## Visualizations

The project includes:
- Elbow Method plot for cluster selection.
- Daily taxi demand visualization.
- ARIMA forecasting visualization.

See the `results/` directory for the figures.

## Future Work

- Explore SARIMA for seasonal demand forecasting.
- Evaluate Random Forest and XGBoost.
- Incorporate weather, holidays, and traffic information.
- Improve demand classification and forecasting performance.
- Explore scalable real-time transportation analytics.


## Research Paper

The project is documented in an IEEE-style research paper.

The paper will be available in the `paper/` directory.

## Author

**Ghada Alsultan**

College of Computer Science  
King Khalid University

## Acknowledgment

NYC Taxi and Limousine Commission for providing publicly accessible taxi trip records.

