# Feature-Engineering

How to predict the number of bike share rentals during a given hour of the day? The task is to engineer some new features to try to improve model's ability

[data source](https://docs.google.com/spreadsheets/d/e/2PACX-1vROUXPkYUkX-2W7JbJ0-oNKaXzpg4NtmU9IeWEY6yFKm32ZEJOpRh_soHD4BeIcuHjYik3SEoXmkgwj/pub?output=csv)

#Result

![image](https://user-images.githubusercontent.com/126204698/235315099-c50b13fe-c44f-4f05-8b49-fe885391edb5.png)

- Engineered data has significant better metrics across the board.

- The most significant one is on R2 test score.

- RMSE scores on Engineered data are half of the UNEngineered data.

#Processes

##Feature Engineering

- Transforming the 'datetime' column into a datetime type and use it to create 3 new columns in the data frame.

-  `.apply()`and a Lambda function are used to convert temperature columns from Celsius to Fahrenheit.

- A new column, 'temp_variance', is created to show if temp is colder or warmer than average temp. 

##Machine Learning - Regression

After identifying target as count, I treat this as a regression dataset and proceed to use bagged tree model on mahcine learning

##Comparison

A comparison on different regression metrics, including RMSE, R2 and others, between original and feature engineered data are presented.
