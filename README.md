1)Credit Card Fraud Detection using Multivariate Gaussian
This repository contains a simple implementation of an anomaly detection approach to identify fraudulent transactions in credit card data. The model fits a multivariate Gaussian distribution on normal transactions and predicts anomalies based on probability thresholds.

2)Dataset
The script uses the well-known creditcard.csv dataset.
It includes principal component features (V1 to V28).

3)How It Works

The script loads the dataset and selects the PCA features.
Preprocessed Data Ensures all features and the target column (Class) are numeric and Handles missing values by filling them with the median.
the the code fits Multivariate Gaussian and Computes the mean vector and covariance matrix on non-fraudulent data (Class == 0).

4)Compute Probabilities

Then the code Calculates the probability density for each transaction and Marks transactions as fraud if the probability is below a chosen threshold (0.3 percentile).

5)Evaluate Performance
Uses F1 Score to measure detection performance.

6)Requirements
Python,NumPy,pandas,scikit-learn and SciPy.
