# Food Sales Prediction

## Predicting sales depending on the store and product features

Mahdi KRIAA

Welcome to this project wich aims to predict food sales based on various factors. In the ever-evolving world of retail and food service, understanding sales patterns is crucial for business planning and growth. The project focuses on leveraging analytical and modeling techniques to forecast food sales. The used dataset includes information such as the type of food, price, location of sale, promotional details, and historical sales data. The goal is to build a model that can accurately predict future sales, helping businesses to manage inventory, optimize supply chain processes, and ultimately increase profitability. We’ll be exploring different machine learning algorithms, data preprocessing techniques, and feature engineering methods to achieve this.

## Data Source: 
Food sales history
https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view

For this dataset, there were 8523 rows and 12 columns.

## Data Dictionary

<p align = "center"> 
  <img src = https://github.com/Mahdi-Kriaa/food_sales_prediction/blob/main/Images/data_dictionary.PNG>
</p>


## To prepare this data, the data was cleaned, and the following processes were performed:

### Exploratory Data Analysis
    - During the exploratory data analysis, a boxplot and histogram was visualized for each numeric datatype column. 
    - Also, a boxplot was visualized for each categorical column. 
    

<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/food_sales_prediction/blob/main/Images/sales_boxplot.png">
</p>

This histogram shows that the majority of the sales are less than $6,200.


 ### Expanatory Data Analysis
    - To visualize the data for explantory purposes, a barplot and regplot were chosen.
    - The barplot xas chosen to show how the types affect sales. 
    - Finally, a regplot was chosen to show the trend of sales over the item MRP depending on the outlet type.


## Explanatory Visuals

<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/food_sales_prediction/blob/main/Images/ItemType_VS_Sales.png">
</p>


We notice that the item type has not a significant impact on the sales


<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/food_sales_prediction/blob/main/Images/ItemMRP_VS_Sales.png">
</p>


We see that The item MRP and sales are almost linearly correlated for each outlet type


 ### Maching Learning Using the Following Models:
    - Linear Regression Model
    - Tuned Decision Tree Regressor Model
    
## Models Evaluated & Results

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

Sales Insights

To increase the sales of the store, the saler must primarily choose the optimal store's features.

Model Performance

The tuned decision tree model is better than the linear regression model but, considering the previous regression metrics from how the model performed, using it to make predictions about sales of a product in a specific store would not be a very reliable. in fact the error presented by the RMSE score cannot be ignored.



## For Further Information

For any additional questions, please contact:
- Mahdi KRIAA
- mahdikriaa@gmail.com
