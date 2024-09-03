# **House Price Prediction Project Report**

## **1. Introduction**

The primary goal of this project was to develop a simple linear regression model to predict house prices based on various features, including the number of bedrooms, square footage, and other relevant attributes. The accuracy of the model is essential for stakeholders in the real estate market, such as buyers, sellers, and agents, to make informed decisions.

## **2. Dataset Overview**

The dataset used consists of 13 features, including `price`, `area`, `bedrooms`, `bathrooms`, `stories`, `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `parking`, `prefarea`, and `furnishingstatus`. These features represent the key aspects that typically influence house prices.

## **3. Model Evaluation**

The model's performance was evaluated using the following metrics:

- **Mean Absolute Error (MAE)**: 970,043.40
- **Mean Squared Error (MSE)**: 1,754,318,687,330.67
- **R² Score**: 0.6529

These results indicate that the model explains approximately 65.3% of the variance in house prices, with an average prediction error of around $970,000. The large MSE suggests that there may be significant variance in the prediction errors, possibly due to outliers or high-priced properties in the dataset.

## **4. Model Optimization**

To enhance the model's accuracy, regularization techniques were applied:

### **4.1 Ridge Regression**

- **Best Parameters**: `alpha = 10`
- **Best R² Score**: 0.6485

Ridge regression helped to mitigate overfitting by penalizing large coefficients, slightly improving the model's robustness.

### **4.2 Lasso Regression**

- **Best Parameters**: `alpha = 100`
- **Best R² Score**: 0.6470

Lasso regression further improved model performance by performing feature selection, setting some coefficients to zero, and thus simplifying the model.

## **5. Conclusion**

The linear regression model, enhanced with Ridge and Lasso regularization, performed reasonably well, explaining about 65% of the variance in house prices. However, there is still room for improvement, particularly in reducing the error margins. Future work could explore non-linear models, additional features, and more sophisticated data preprocessing techniques to further improve prediction accuracy.
