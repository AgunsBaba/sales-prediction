## Introduction
This project is my attempt to build and evalute two models (Linear Regression and Decision Tree Regression) on the popular [BigMart Sales Prediction dataset](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/) to predict the sales from various BigMart stores.

## Data Analysis and Insight
The data for this project contains about 8500 rows and 12 columns. It represents sales data for 1559 unique products taken from 10 stores of various sizes across the country. I performed various data pre-processing tasks to make the dataset ready for model fitting. Preliminary analysis of the data showed that the independent variables in the dataset do not have very strong correlation with the dependent variable (Item_Outlet_Sales). The correlation matrix is show below.

                                 
![image](https://user-images.githubusercontent.com/15455064/143792990-3894c9f5-e71f-409d-a061-ba2bbc0d4eb9.png)
![image](https://user-images.githubusercontent.com/15455064/143792963-f9408034-4ad6-4723-a2ac-4099fc8e295e.png)

## Model Building and Evaluation
As I mentioned above, a linear regression model and a decision tree regression model were built to predict the product sales. The perdormance of both models is as shown below



![image](https://user-images.githubusercontent.com/15455064/143793172-f648eccc-3b03-4214-abd1-ec8b7bdf4a00.png)
![image](https://user-images.githubusercontent.com/15455064/143793242-86678c0d-6b27-4976-94e3-ebab2d7b7158.png)

## Conclusion
Based on the metrics for the models, it is obvious that the Decision Tree Regression model is better.

From the model metrics, the RMSE of the decision tree model at USD1027.74 is lower than that of the linear regression model at USD1070.95. This means that the deviation of the predicted values from the actual values is smaller and therefore better with the decision tree model than with the linear regression model. 

Additionally, the R2 score on the test set for the decision tree model at 0.611 is higher than that of the linear regression model at 0.578. This means that decision tree model does a better job of explaining the variability in sales (target variable) given the independent variables than the linear regression model.

