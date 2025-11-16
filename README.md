# MSCS_634_Lab_4
# Prasanna Adhikari
# Diabetes Disease Progression Prediction - Regression Models
# 17.11.2025
## Purpose of the Lab Work

This lab explores the performance of various regression models in predicting the progression of diabetes using a dataset from sklearn. The primary aim is to evaluate and compare the following models: Linear Regression, Multiple Regression, Polynomial Regression, Ridge Regression, and Lasso Regression. The goal is to assess the accuracy, behavior, and potential for overfitting of each model. The dataset contains several health-related features of diabetic patients, and the target variable is the disease progression that we aim to predict.

## Models Implemented

### Linear Regression
Linear Regression is a simple model that assumes a linear relationship between the input features and the target variable. This model can handle both single and multiple input features to predict the outcome.

### Multiple Regression
Multiple Regression is an extension of Linear Regression that incorporates multiple input features to predict the target variable. This model allows for a more nuanced understanding of the relationship between the features and the target.

### Polynomial Regression
Polynomial Regression extends Linear Regression by introducing polynomial features to capture non-linear relationships in the data. It is useful for modeling more complex patterns that simple linear regression cannot capture.

### Ridge Regression
Ridge Regression is a variation of Linear Regression that uses L2 regularization to prevent overfitting. By applying a penalty to the magnitude of coefficients, this model helps improve generalization, especially when dealing with multicollinearity.

### Lasso Regression
Lasso Regression also modifies Linear Regression but uses L1 regularization, which not only helps prevent overfitting but also performs feature selection by driving some coefficients to zero, focusing only on the most important features.

## Model Evaluation and Results

### Linear Regression
- **R²**: 0.233  
- **MAE**: 52.26  
- **RMSE**: 63.73  

Linear Regression performed poorly with a low R² value, indicating that it only explained 23.3% of the variance in the target variable. The MAE and RMSE values suggest significant errors in the predictions.

### Multiple Regression
- **R²**: 0.453  
- **MAE**: 42.79  
- **RMSE**: 53.85  

Multiple Regression showed an improvement over Linear Regression, explaining 45% of the variance in the target variable. The MAE and RMSE values were lower compared to Linear Regression, indicating better predictive accuracy.

### Polynomial Regression
- **R²**: 0.233  
- **MAE**: 52.18  
- **RMSE**: 63.75  

Polynomial Regression produced similar results to Linear Regression, with no significant improvement in the performance metrics. The model showed a tendency for overfitting, especially at higher polynomial degrees, leading to similar errors in predictions.

### Ridge Regression
- **R²**: 0.419  
- **MAE**: 46.14  
- **RMSE**: 55.47  

Ridge Regression showed a better performance than Linear and Polynomial Regression by incorporating L2 regularization. While it was not the top performer, it did help mitigate overfitting, leading to better generalization.

### Lasso Regression
- **R²**: 0.472  
- **MAE**: 42.85  
- **RMSE**: 52.90  

Lasso Regression outperformed all other models, achieving the highest R² value and the lowest MAE and RMSE. Its ability to perform feature selection alongside regularization helped prevent overfitting and improved the model’s accuracy.

## Key Insights

- **Lasso Regression** demonstrated the best performance overall, showing the highest R² and the lowest error metrics, while also effectively handling overfitting.
- **Multiple Regression** and **Ridge Regression** improved upon Linear and Polynomial Regression by incorporating more features and applying regularization techniques.
- **Polynomial Regression** showed a risk of overfitting, especially with higher-degree polynomials, and did not provide any significant improvement over the simpler Linear Regression model.
- The results highlight the importance of **regularization** (Ridge and Lasso) in preventing overfitting and improving model performance.

## Conclusion

In this lab, various regression models were applied to predict the progression of diabetes using the provided dataset. **Lasso Regression** emerged as the best-performing model due to its ability to prevent overfitting and perform feature selection. **Ridge Regression** and **Multiple Regression** also demonstrated improvements over the simpler Linear and Polynomial Regression models. The findings emphasize the critical role of regularization techniques, such as Ridge and Lasso, in enhancing model performance, reducing overfitting, and ensuring better generalization in predictive modeling tasks.
