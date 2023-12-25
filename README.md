# Food Sales Prediction

## Project Description
This project aim to predict food sales based on various factors. In the ever-evolving world of retail and food service, understanding sales patterns is crucial for business planning and growth. The project focuses on leveraging analytical and modeling techniques to forecast food sales. The used dataset includes information such as the type of food, price, location of sale, promotional details, and historical sales data. The goal is to build a model that can accurately predict future sales, helping businesses to manage inventory, optimize supply chain processes, and ultimately increase profitability. We’ll be exploring different machine learning algorithms, data preprocessing techniques, and feature engineering methods to achieve this.

## Data

### Data Source: 
Food sales history
https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view

For this dataset, there were 8523 rows and 12 columns.

### Data Dictionary

<p align = "center"> 
  <img src = https://github.com/Mahdi-Kriaa/food_sales_prediction/blob/main/Images/data_dictionary.PNG>
</p>

## Methodology

We will employ various data preprocessing techniques to handle missing values and categorical variables. We will explore different machine learning models, including random forests and gradient boosting, to predict the sales for each store. Model performance will be evaluated based on different metrics such as r2 and RMSE.

## Exploratory Data Analysis

To explore the dataset the following plots were used:

    - a boxplot and histogram was visualized for each numeric datatype column. 
    - a boxplot was visualized for each categorical column.
    - a contingincy matrix for some categorical column
    

<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/food_sales_prediction/blob/main/Images/sales_boxplot.png">
</p>

This histogram shows that the majority of the sales are less than $6,200.
 
To visualize the data for explantory purposes, a barplot and regplot were chosen.

    - the barplot was chosen to show how the types affect sales. 
    - the regplot was chosen to show the trend of sales over the item MRP depending on the outlet type.

<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/food_sales_prediction/blob/main/Images/ItemType_VS_Sales.png">
</p>


We notice that the item type has not a significant impact on the sales


<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/food_sales_prediction/blob/main/Images/ItemMRP_VS_Sales.png">
</p>


We see that The item MRP and sales are almost linearly correlated for each outlet type

## Machine Learning 

### Machine Learning Models

    - Linear Regression Model
    - Tuned Decision Tree Regressor Model
    
### Models Evaluation & Results

- Linear Regression Model (Testing Set):
  - R^2: 0.567277
  - RMSE: 1100.93

- Decision Tree Regressor Model (Testing Set):
  - R^2: 0.597148
  - RMSE: 1062.25


- The Final Model Chosen was a `Tuned Decision Tree Regressor Model` with the max_depth tuned to 5.
- For the testing set on the model, `59.7%` of the variance in y was explained by x. 
- The Root Mean Squared Error had a calculation of `$1,062.25`.

## Recommendations

- To increase the sales of the store, the saler must primarily choose the optimal store's features.
- The tuned decision tree model is better than the linear regression model but, considering the previous regression metrics from how the model performed, using it to make predictions about sales of a product in a specific store would not be a very reliable. in fact the error presented by the RMSE score cannot be ignored.



