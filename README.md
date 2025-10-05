# Retail Price Forecasting

This project aims to forecast **retail shelf prices** using historical data.  
Several machine learning models such as **RandomForest, XGBoost, and LightGBM** are trained and compared to minimize the error (RMSE) and improve forecasting accuracy.  

---

## Dataset
- **train.csv**: Contains historical product price data used for training.  
- **test.csv**: Contains unseen data for prediction.  
- Target column: `product_price`  
- Features include:
  - Date (transformed into month & year)  
  - Numerical features (e.g., sales, costs, discounts, etc.)  
  - Categorical features (e.g., product type, store, category, etc.)  

---

## Methods
1. **Data Preprocessing**
   - Date column converted into `month` and `year`.  
   - Missing values filled with median (numerical) or mode (categorical).  
   - Features scaled and categorical variables one-hot encoded.  

2. **Models Used**
   - RandomForestRegressor  
   - XGBRegressor (XGBoost)  
   - LGBMRegressor (LightGBM)  

3. **Evaluation Metric**
   - Root Mean Squared Error (**RMSE**)  
   - Lower RMSE indicates better performance.  

---

## Results
- Model performances are compared on validation data.  
- A bar plot is generated showing **RMSE scores** of each model.  
- The best-performing model is selected automatically for predictions on the test dataset.  

