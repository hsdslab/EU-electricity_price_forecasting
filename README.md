# Artificial Intelligence-Based Modelling of European Electricity Prices Using SHAP Values

This repository contains supplementary codes and datasets for the scientific article titled *"Artificial Intelligence-Based Modelling of European Electricity Prices Using SHAP Values Based on Open-Source Data and Models"*.

[link to the article]

## Repository Structure

### `source/processing`
- [**`dataproc.ipynb`**](./source/processing/dataproc.ipynb): 
  - Code for creating standardized data from ENTSO-E datasets
  - Frequency standardization to hourly
  - Feature extraction
  - Missing value handling
- [**`data_lag.ipynb`**](./source/processing/data_lag.ipynb):
  - Code for creating lagged input and output datasets for model training from the standardized data

### `source/models`
- **`cb_optuna.ipynb`**:
  - CatBoost hyperparameter optimization, training, and evaluation
  - Covers the two time periods described in the article
  - Uses inputs and outputs created with [`data_lag.ipynb`](./source/processing/data_lag.ipynb)
- **`dnn_optuna.ipynb`**:
  - Same as above, implemented with a deep neural network
- **`rf_optuna.ipynb`**:
  - Same as above, implemented with a random forest
- **`svm_optuna.ipynb`**:
  - Same as above, implemented with a support vector machine

## Data
Collected data is available at: [link]
