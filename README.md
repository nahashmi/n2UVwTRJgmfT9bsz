**Background**

In this project, a Machine Learning algorithm has been developed to predict if a bank's customer will subscribe to their term deposit offer or not. The prediction model used the bank's call center data of 40000 calls made to the customers and made predictions on the likelihood of customers to opt for the term deposit depending on different variables like the customer's age, job, balance etc. 

**Solution**

The solution to this requirement is a predictive model (XGBoost) based on the available data of 40,000 calls made to the customers. This dataset was split between TRAIN and TEST datasets (80/20). Before model development, Exploratorty Data Analysis (EDA) was performed to handle missing/NULL values and OUTLIERS and the relationship of the Y variable against each X variable was plotted to assess the relevance of X variables and then dropping the ones that were not found much relevant. 

Since this data also contained categorical variables, so ONE-HOT ENCODING was used to assign an order to the categorical variables and to find OUTLIERS. The concepts of 'Bins' was also used to handle the continuous numerical variables. 

Initially, the performance of model was low for the positive results (1s) as indicated by the RECALL parameter in the Classification Report. Therefore, different sampling weights were tried in the XGBoost model to optimize the results and a weight of 10 was found to strike a decent trade-off between the RECALL value and the overall performance of the model. 
