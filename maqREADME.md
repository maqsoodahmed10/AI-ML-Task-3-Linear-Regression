# Task 3: Linear Regression - House Price Prediction

## Project Overview
This project implements Simple and Multiple Linear Regression models using Python, Pandas, and Scikit-Learn to analyze and predict house prices.

## Repository Structure
- `clean data/`: Contains the Jupyter Notebook (`cleaneddata.ipynb`)
- `raw data/`: Raw dataset file
- `images/`: Visualizations including actual vs. predicted values (`regression_plot.png`)

## Results & Plot
![Regression Line Output](images/regression_plot.png)

---

## Interview Questions & Answers

### 1. What assumptions does linear regression make?
- **Linearity:** Linear relation between features and target.
- **Independence:** Residuals (errors) are independent of each other.
- **Homoscedasticity:** Constant variance of residuals.
- **Normality:** Residuals follow a normal distribution.
- **No Multicollinearity:** Independent variables aren't highly correlated.

### 2. How do you interpret the coefficients?
Each coefficient represents the expected change in the target variable for a one-unit change in that specific predictor, holding all other variables constant.

### 3. What is R² score and its significance?
The $R^2$ score (coefficient of determination) measures the proportion of variance in the target variable explained by the input features. It ranges from 0 to 1 (higher is better).

### 4. When would you prefer MSE over MAE?
Prefer **MSE** when large errors/outliers are especially undesirable and need to be heavily penalized (since MSE squares the error terms).

### 5. How do you detect multicollinearity?
By calculating the **Variance Inflation Factor (VIF)** or using a **correlation matrix heatmap**. A VIF > 5-10 indicates high multicollinearity.

### 6. What is the difference between simple and multiple regression?
- **Simple Linear Regression:** Uses 1 independent feature to predict $y$.
- **Multiple Linear Regression:** Uses 2 or more independent features to predict $y$.

### 7. Can linear regression be used for classification?
No. Linear regression outputs unbounded continuous values rather than probabilities between 0 and 1, making it unsuitable and sensitive to outliers for classification tasks.

### 8. What happens if you violate regression assumptions?
It can lead to biased coefficient estimates, invalid standard errors, inaccurate confidence intervals, and unreliable predictions.
