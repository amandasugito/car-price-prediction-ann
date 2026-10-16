# 🚗 Car Price Prediction Using Artificial Neural Networks (ANN)

## 📌 Project Overview
This project focuses on predicting car selling prices using Artificial Neural Networks (ANN). The workflow includes data preprocessing, exploratory data analysis (EDA), feature engineering, model development, and performance evaluation.

Two ANN models are implemented and compared: a baseline model using sigmoid activation and an improved model using ReLU activation.

## 🎯 Objectives
- Understand the structure and characteristics of the car dataset.
- Perform data cleaning and feature engineering.
- Prepare numerical and categorical features for neural network modeling.
- Build and train an ANN model using sigmoid activation.
- Improve the model using ReLU activation.
- Evaluate and compare model performance using R², RMSE, and MAE.

## 🧹 Data Preprocessing
The notebook includes the following preprocessing steps:
- Inspecting dataset structure, descriptive statistics, and missing values.
- Removing a row with a missing `selling_price`.
- Converting `mileage` into a numerical format.
- Extracting torque and RPM information from the `torque` column.
- Encoding categorical features using Label Encoding.
- Standardizing input features and the target variable.

## 📊 Exploratory Data Analysis
The dataset is explored using:
- Descriptive statistics.
- Selling price distribution.
- Correlation heatmap.
- Torque versus selling price scatterplot.

## 🧠 Model Development

### Baseline Model — Sigmoid
- Three hidden layers with 512, 256, and 128 neurons.
- Sigmoid activation in the hidden layers.
- Batch Normalization and Dropout.
- Adam optimizer with a learning rate of 0.001.
- Mean Squared Error (MSE) loss.
- 20 training epochs with a batch size of 32.

### Improved Model — ReLU
- Three hidden layers with 512, 256, and 128 neurons.
- ReLU activation in the hidden layers.
- Batch Normalization and Dropout.
- Adam optimizer with a learning rate of 0.0005.
- Mean Squared Error (MSE) loss.
- 20 training epochs with a batch size of 24.

## 📈 Model Evaluation
The notebook reports the following test-set results:

| Metric | Sigmoid | ReLU |
|---|---:|---:|
| R² | 0.8274 | 0.8582 |
| RMSE | 3567.86 | 3233.57 |
| MAE | 1851.19 | 1779.18 |

Based on the reported results, the ReLU model performs better across all three metrics, with a higher R² and lower RMSE and MAE.

## 📂 Project Files
- `car_price_prediction.ipynb` — notebook containing the analysis, preprocessing, model training, and evaluation.
- `2B.parquet` — dataset used in the notebook.

## 🛠️ Tools & Technologies
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook
- Parquet

## 👤 Author
**Amanda Sugito**

Deep Learning academic project at BINUS University.

## 🔗 Connect with Me
- LinkedIn: Amanda Sugito | www.linkedin.com/in/amanda-sugito
- GitHub: amandasugito | https://github.com/amandasugito

## ⚠️ Disclaimer
This project was developed for educational purposes. The reported model evaluation metrics reflect the results recorded in the notebook.
