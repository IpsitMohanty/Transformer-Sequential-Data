# Transformer-Based Stock Price Prediction

This repository contains the implementation and experiments with a Transformer-based deep learning model for predicting stock prices using sequential data. The project demonstrates the application of Transformer architectures for time-series forecasting, with a focus on exploring different configurations and optimizations.

---

## Project Overview

The goal of this project is to apply Transformer models to predict stock prices using sequential data. The repository includes the following features:
- **Data Preparation:** Synthetic stock price data generation and preprocessing.
- **Model Architecture:** Implementation of a Transformer model with:
  - Multi-Head Self-Attention
  - Feed-Forward Neural Networks
  - Residual Connections and Layer Normalization
- **Hyperparameter Tuning:** Experiments with different batch sizes, activation functions, and dropout rates.
- **Training and Evaluation:** Training the model with various configurations and visualizing predictions.

---

## Features

### 1. **Synthetic Data Generation**
- Creates synthetic stock price data with trends and random noise.
- Normalizes data using MinMaxScaler.
- Prepares data for training using a sliding window approach.

### 2. **Model Architecture**
- Implements a Transformer model with:
  - Custom `MultiHeadSelfAttention` and `TransformerBlock` layers.
  - Stacked encoder layers for sequential data processing.
  - Dropout for regularization.
- Supports configurable hyperparameters such as embedding dimension, number of heads, and feed-forward dimensions.

### 3. **Training and Evaluation**
- Trains the Transformer model on synthetic stock price data.
- Evaluates the model using loss metrics and visualizations.
- Experiments with:
  - Batch sizes (e.g., 16 and 64)
  - Activation functions (`ReLU` and `tanh`)
  - Dropout rates.

### 4. **Visualization**
- Plots training and validation loss to evaluate model performance.
- Compares true stock prices with model predictions.

---

## Repository Structure

```plaintext
├── data/
│   ├── stock_prices.csv          # Synthetic stock price data
├── models/
│   ├── transformer_model.py      # Implementation of Transformer architecture
├── notebooks/
│   ├── stock_price_prediction.ipynb  # Jupyter notebook with experiments
├── results/
│   ├── loss_comparison.png       # Visualization of training and validation loss
│   ├── predictions_vs_actual.png # Comparison of true data and predictions
├── README.md                     # Project documentation
