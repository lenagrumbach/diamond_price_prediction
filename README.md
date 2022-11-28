## Project:  diamond_price_prediction
  Project status (Completed)
  
## Project Description
  In this project I'm going to work with data to understand the characteristics of a diamond that are most likely to influence its price. 
  
## Project objective
  My goal is to create a prediction to estimate the price of 5000 diamonds achieving an average error less than 900 dollars.
  
## Technologies 
  - Python
  - Pandas
  - Sklearn.linear_model
  - Sklearn.ensemble
  - Matplotlib
  - Seaborn

## Steps
  - Exploratory data analysis (EDA)
  - Data cleaning
  - Linear Regression
  - Random Forest Regression
  
## **Conclusion**

Prediction with Random Forests regression using variables 'carat', 'x', 'y', 'z', 'cut', 'color', 'clarity', 'table', RMSE = 543.5631396740744 dollars

website to check price estimate, https://daft-oct2020-rick-diamonds.herokuapp.com

## Version Prediction documentation

  - Prediction with historical average price, RMSE = 3980.713882502374

  - Prediction with historical price median, RMSE = 4255.533080942974

  - Prediction with simple linear regression model using the variable 'carat', RMSE = 1605.15175707362

  - Prediction with multiple linear regression model using variables 'carat' and 'cut', RMSE = 1578.5538450152076 (a negative value, -201.82, appeared in the column 'price_predicted')

**Results with low values correction**:

  - Prediction with multiple linear regression model using variables 'carat' and 'cut', RMSE = 1560.3875526620348

  - Prediction with multiple linear regression model using variables 'carat', 'cut' and 'color', RMSE = 1494.3832889738444

  - Prediction with multiple linear regression model using variables 'carat', 'cut', 'color' and 'clarity', RMSE = 1226.9362366819055

  - Prediction with multiple linear regression model using variables 'carat', 'cut', 'color', 'clarity' and 'x', RMSE = 1240.4099341776305

**Results after drop 18 rows with value 0 in columns 'x', 'y' or 'z' (18 out of 48940):**

  - Prediction with multiple linear regression model using variables 'carat', 'cut', 'color', 'clarity' and 'x', RMSE = 1242.9898663407414

  - Prediction with multiple linear regression model using variables 'carat', 'cut', 'color', 'clarity', 'x' and 'y', RMSE = 1242.601308595802

  - Prediction with multiple linear regression model using variables 'carat', 'cut', 'color', 'clarity', 'x', 'y' and 'z', RMSE = 1243.017142456451

  - Prediction with multiple linear regression model using variables 'carat', 'cut', 'color' and 'clarity', RMSE = 1227.0395614594963

**Drop the 18 rows didn't bring better results, so undo it.**

  - Prediction with multiple linear regression model using variables 'carat', 'cut', 'color' and 'clarity', RMSE = 1226.9362366819055

**Filter on carat size (model applied to all df_rick_diamonds):**
  
  **Carat greater than or equal to the median:**

  - Prediction with multiple linear regression model using variables 'carat', 'cut', 'color', 'clarity', 'x', 'y' and 'z', RMSE = 1120.951108234914

  - Prediction with multiple linear regression model using variables 'carat', 'color', 'clarity', 'x', RMSE = 1119.051685118186
  
  **Carat greater than or equal to 90% of the median:**
  
  Best model so far: Prediction with multiple Linear Regression model using variables 'carat', 'x', 'y', 'z', 'cut', 'color', 'clarity', RMSE = 1115.2815460356976

  Prediction with **Random Forests Regression** using variables 'carat', 'x', 'y', 'z', 'cut', 'color', 'clarity', 'table', **RMSE = 543.5631396740744**
