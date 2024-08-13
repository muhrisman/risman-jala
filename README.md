# Shrimp Farming Forecast Dashboard

## Overview

The Shrimp Farming Forecast Dashboard is designed to provide predictions on various aspects of shrimp farming based on environmental and operational inputs. The dashboard predicts survival rate, average body weight, biomass, and projected revenue, aiding in decision-making and operational planning.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.6 or newer
- pip (Python package installer)

### Installation

   1. **Clone the Repository**

      ```bash
      git clone https://github.com/muhrisman/risman-jala.git
      cd risman-jala

   2. **Set up a Python Virtual Environment**
      ```bash
      python -m venv shrimp_env
      shrimp_env\Scripts\activate

   3. **Install Required Packages**
      ```bash
      pip install -r requirements.txt

   Alternatively, if a requirements.txt file is not provided, install the dependencies directly:

      ```bash
      pip install dash numpy plotly joblib

### Usage

   To run the dashboard locally, execute the following command in the terminal:

      ```bash
      python app.py

This command starts the server. You can then access the dashboard by navigating to http://127.0.0.1:8050/ in your web browser.

### Features

- **Interactive Inputs**: Customize parameters such as the number of days until harvest, seed count, pond area, feed quantity, and various environmental conditions directly through the interface.
- **Real-time Predictions**: The dashboard updates its predictions on survival rates, body weight, biomass, and revenue in real-time as input parameters are adjusted.
- **Graphical Displays**: Each metric is visualized through dynamic graphs that adjust according to the input changes, allowing for immediate visual analysis and decision-making.

## Models

The dashboard utilizes two primary machine learning models:
- **Survival Rate Model (`model_sr.pkl`)**: Predicts the survival rate of shrimp based on environmental factors and farming practices over time.
- **Average Body Weight Model (`model_abw.pkl`)**: Estimates the average body weight of shrimp throughout the farming cycle.

These models are pre-trained and loaded into the application using the `joblib` library. Ensure that these model files are located in the project directory or appropriately link to their paths in the script.

