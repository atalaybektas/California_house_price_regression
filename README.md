# 🏠 California Housing Price Prediction with PySpark

This project demonstrates a scalable machine learning pipeline using **Apache Spark (PySpark)** to predict median house values in California. It covers the entire data science workflow, including data cleaning, feature engineering, model training, and evaluation — all within a distributed computing framework.

---

## 📌 Project Overview

- **Objective:** Predict `median_house_value` using a linear regression model built with Spark MLlib.
- **Tools:** PySpark (Spark MLlib), Pandas, Matplotlib
- **Dataset:** [California Housing Prices - Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices)

---

## 🔍 Steps & Pipeline

1. **Data Loading:**  
   Read CSV data into a Spark DataFrame using `spark.read.csv()`

2. **Data Cleaning:**  
   - Handling missing values in `total_bedrooms` by filling with mean  
   - Removing outliers from `total_rooms` using the IQR method

3. **Data Preprocessing:**  
   - Converting categorical `ocean_proximity` to numeric using `StringIndexer`  
   - Combining features using `VectorAssembler`

4. **Train-Test Split:**  
   Splitting the dataset randomly (80% training, 20% test)

5. **Model Training:**  
   Training a **Linear Regression** model with the selected features

6. **Model Evaluation:**  
   Calculating:
   - Root Mean Squared Error (RMSE)
   - Mean Absolute Error (MAE)
   - R² Score  
   Visualizing predictions vs true values using Matplotlib

---

## 📊 Example Output

