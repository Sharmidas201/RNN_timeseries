# Time Series Prediction with Recurrent Neural Network

This code example demonstrates how to use a recurrent neural network (RNN) to solve a time series prediction problem, specifically forecasting book sales based on historical values. The code is adapted from Chapter 9 of the book "Learning Deep Learning" by Magnus Ekman (ISBN: 9780137470358), focusing on the section "Programming Example: Forecasting Book Sales".

## Overview
The code initializes and trains an RNN model using PyTorch to predict future book sales. It includes data preprocessing, model training, evaluation, and comparison with a naive prediction approach.

## Initialization and Data Preparation
The code begins with importing necessary modules and loading the sales data from a CSV file. The data is split into training and test sets. The historical sales data is then plotted to visualize patterns and trends.

## Model Training
The RNN model is defined and trained using the training data. The model architecture consists of an RNN layer followed by a custom layer to retrieve the last timestep output, and a linear layer for prediction. Training involves optimizing the model parameters to minimize the mean squared error loss.

## Naive Prediction Comparison
A naive prediction approach, where tomorrow's sales are predicted to be the same as today's, is implemented for comparison. The naive predictions are evaluated using mean squared error (MSE) and mean absolute error (MAE) on the test data.

## Results Visualization
The final validation results (MSE and MAE) of the trained model and the naive testing results are compared through bar plots. Additionally, the training data columns are plotted to visualize individual features.

## Predictions and Visualization
The trained model is used to predict book sales on the test data, and the predictions are plotted alongside the actual sales data for visualization. The predictions are de-standardized to represent actual sales values.

For detailed explanations and discussions, refer to Chapter 9 of the book "Learning Deep Learning" by Magnus Ekman.
