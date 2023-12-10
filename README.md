# DeepTradeInsights


This project implements a Stock Price Predictor using a Long Short-Term Memory (LSTM) model. The model is trained on historical stock price data and can make predictions for future stock prices.

## Overview

The Stock Price Predictor leverages deep learning techniques, specifically LSTM neural networks, to analyze historical stock price data and make predictions for future stock prices. This README provides an overview of the project, instructions for setup, and details on how to use the predictor.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Training the Model](#training-the-model)
  - [Making Predictions](#making-predictions)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [License](#license)

## Getting Started

### Prerequisites

Before you begin, ensure you have the following prerequisites:

- Python 3.x
- Pip (Python package installer)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/stock-price-predictor.git
    ```

2. Navigate to the project directory:

    ```bash
    cd stock-price-predictor
    ```

3. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Training the Model

To train the LSTM model, follow these steps:

1. Prepare your stock price dataset in CSV format. Ensure it contains at least the 'Date' and 'Close' columns.

2. Run the training script:

    ```bash
    python train_model.py --data_path path/to/your/dataset.csv
    ```

3. The trained model will be saved to the 'models' directory.

### Making Predictions

To make stock price predictions, follow these steps:

1. Use the trained model for prediction:

    ```bash
    python predict.py --model_path models/your_model.h5 --data_path path/to/your/test_data.csv
    ```

2. The predictions will be displayed, and a plot of actual vs. predicted prices will be saved.

## Project Structure
- **data:** Contains the stock price dataset.
- **models:** Directory to save trained models.
- **train_model.py:** Script for training the LSTM model.
- **predict.py:** Script for making predictions using the trained model.
- **utils:** Utility functions for data processing and visualization.
- **tests:** Directory for unit tests.

## Dependencies

- numpy
- pandas
- matplotlib
- scikit-learn
- keras
- streamlit
- prophet


Install dependencies using:

```bash
pip install -r requirements.txt
