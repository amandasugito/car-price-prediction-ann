# 🚗 Car Price Prediction Using Artificial Neural Networks

## 📌 Project Overview
This project explores car price prediction using Artificial Neural Networks (ANN). It covers data inspection, data cleaning, feature engineering, exploratory data analysis (EDA), model development, and performance evaluation.

Two ANN models are compared: a baseline model using sigmoid activation and an improved model using ReLU activation.

## 🎯 Objectives
- Analyze and clean the car dataset before modeling.
- Handle missing values and inconsistent data types.
- Prepare numerical and categorical features for ANN.
- Build an ANN with three hidden layers using sigmoid activation.
- Improve the model architecture using ReLU activation.
- Compare model performance using R², RMSE, and MAE.

## 🧹 Data Preprocessing
The preprocessing workflow includes:
- Inspecting dataset structure, descriptive statistics, and missing values.
- Removing the row with a missing `selling_price`.
- Converting `mileage` into a numerical format.
- Extracting torque values and RPM information from the `torque` column.
- Encoding categorical features using Label Encoding.
- Standardizing input features and the target variable.

## 📊 Exploratory Data Analysis
The notebook explores the dataset through:
- Descriptive statistics.
- Selling price distribution.
- Correlation heatmap.
- Torque versus selling price scatterplot.

## 🧠 Model Development
### Baseline Model — Sigmoid
- Three hidden layers: 512, 256, and 128 neurons.
- Sigmoid activation in the hidden layers.
- Batch Normalization and Dropout.
- Adam optimizer with a learning rate of 0.001.
- Mean Squared Error (MSE) loss.
- Training for 20 epochs with a batch size of 32.

### Improved Model — ReLU
- Three hidden layers: 512, 256, and 128 neurons.
- ReLU activation in the hidden layers.
- Batch Normalization and Dropout.
- Adam optimizer with a learning rate of 0.0005.
- Mean Squared Error (MSE) loss.
- Training for 20 epochs with a batch size of 24.

## 📈 Model Evaluation
The notebook reports the following test-set results:

| Metric | Sigmoid | ReLU |
|---|---:|---:|
| R² | 0.8274 | 0.8582 |
| RMSE | 3567.86 | 3233.57 |
| MAE | 1851.19 | 1779.18 |

Based on the reported metrics, the ReLU model performs better across all three evaluation metrics, with a higher R² and lower RMSE and MAE.

## 📂 Project Files
- `car_price_prediction.ipynb` — notebook containing the analysis and ANN models.
- `2B.parquet` — dataset used in the notebook.

## 🛠️ Tools & Libraries
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook
- Parquet

## 👤 Project Context
An academic Deep Learning assignment covering dataset analysis, ANN implementation, model improvement, and evaluation.

## ⚠️ Disclaimer
This project is for educational purposes. The reported evaluation metrics are based on the results recorded in the notebook.
