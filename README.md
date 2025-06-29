#  California Housing Price Prediction with PySpark

- **Objective:** Predict `median_house_value` using regression models built with Spark MLlib.
- **Tools:** PySpark (Spark MLlib), Pandas, Matplotlib
- **Dataset:** [California Housing Prices - Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices)

## Steps & Pipeline

1. **Data Loading:**  
   Read CSV data into a Spark DataFrame using `spark.read.csv()`

2. **Data Cleaning:**  
   - Handling missing values in `total_bedrooms` by filling with mean  
   - Removing outliers from `total_rooms` using the IQR method

3. **Data Preprocessing:**  
   - Converting categorical `ocean_proximity` to numeric using `StringIndexer`  
   - Combining features using `VectorAssembler`


4. **Model Training:**  
   Training a **Linear Regression**, **RandomForest Regressor** and **Gradiant Boosting**  model with the selected features

5. **Model Evaluation:**  
   - Root Mean Squared Error (RMSE)
   - Mean Absolute Error (MAE)
   - R² Score  
   -Visualizing predictions vs true values using Matplotlib




