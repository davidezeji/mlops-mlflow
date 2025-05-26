# MLflow Model Tracking 

This repository demonstrates how to use MLflow for tracking machine learning experiments and model management. It provides examples of training multiple regression models and logging their metrics and artifacts using MLflow.

## Overview

This project showcases:
- Setting up MLflow tracking server
- Training multiple regression models (Linear Regression, Decision Tree, Random Forest)
- Logging model metrics and artifacts
- Model validation and registration

## Project Structure

- `example-mlflow.py`: Main script demonstrating MLflow integration with multiple regression models
- `validation.py`: Script for validating and listing registered models

## Usage

1. Start the MLflow tracking server:
```bash
mlflow server --host 0.0.0.0 --port 5000
```

2. Run the example script:
```bash
python example-mlflow.py
```

3. To view registered models:
```bash
python validation.py
```

## Features

The example script (`example-mlflow.py`) demonstrates:
- Creating synthetic regression data
- Training multiple models:
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
- Logging metrics:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Error (MAE)
  - R² Score
  - Explained Variance Score
- Model artifact logging
- Experiment tracking

## MLflow UI

Access the MLflow UI by opening your browser and navigating to:
```
http://localhost:5000
```

Here you can:
- View experiment runs
- Compare model metrics
- Download model artifacts
- Track model versions

