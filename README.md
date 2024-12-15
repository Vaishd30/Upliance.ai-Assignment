# Upliance.ai-Assignment
This Document provides a detailed explanation of the steps to merge the given three worksheet in Excel and analyse dataset related to user behavior, cooking preferences and other trends.

# Install Necessary Libraries
1. pandas: pip install pandas
2. numpy: pip install numpy
3. seaborn: pip install seaborn
4. matplotlib: pip install matplotlib

# Importing librairies
1. import pandas as pd
2. import numpy as np
3. import matplotlib.pyplot as plt
4. import seaborn as sns

# Task 1- Merge the three worksheets
1. Import pandas library for loading the Excel file into a dataframe
2. Used concat function to merge all the sheets based on the "User ID" column
3. The merged data is saved in another file named "Updated_Assignment.xlsx" file
4. Manually a few adjustments are done in the new file to get a better understanding of the data

# Task 2- Data Manipulation
1. The new file is loaded to a data frame for further analysis
2. Other libraries including numpy, matplotlib and seaborn are impoted
3. Basic data manipulation functions are performed to get a clear understanding of the data and it's features
4. Null values are found using the "isnull" function and the null values are dropped as they are less in number and do not affect the analysis of data
5. Data types in the file is checked and it is found that the "session Start Time" and "Session End Time" feature is an "object" , hence it is converted to "datetime" format

# Task 3- Data Visualization
1. Relationship between Cooking "Session Duration" and "Orders" is represented using the seaborn plot

![image](https://github.com/user-attachments/assets/1886a15d-e108-43b2-b297-69664cee85cb)

It is observed that there are more number of orders when the cooking duration is 30 minutes, this could be due to various factors , this could be the ideal wait time for customers , this could also mean the food needs this much duration to be cooked properly, this could also mean the competitors take more than this duration and hence this duration is ideal. When the Duration is 20 minutes or lesser the number of orders is lesser , this could mean the food is not cooked properly in this short duration and hence lesser orders.

2. Relationship between Number of orders and Time of Day is represented using a Boxplot

![image](https://github.com/user-attachments/assets/79d902eb-9e72-4d49-ac5d-7c8e21f0e411)

The box represents the Interquartile Range(IQR), it contains the middle 50% of the data from Q1 to Q3. The line within the box representds the median value for total orders for each time of the day.The whiskers extend to the minimum and maximum values within a range(1.5 times of the IQR).There are no outliers as these would be marked as individual points beyond the whiskers.
From the boxplot it is obsereved that during Night the median order is around 10. The IQR ranges from around 8 to 12,the orders range from 7 to 14 showing moderate variability.
It is obsereved that the orders are the highest during the morning with median value of 12 and IQR ranges from 10 to 14, the whiskers indicate higher variability, as orders range from 8 to 15.  During the rest of the day the median orders are 9  while the IQR is narrower(7 to 9.5), the whiskers show that total orders range from 5 to 10.

3. Relationship between Total orders and Dish Name using bar Graph

![image](https://github.com/user-attachments/assets/ed61fd42-b7ba-4bfc-a3e6-9f4e3fa0eb48)

From this bar graph the top 5 Dishes are identified, It is observed that Spaghetti is the most popular dish with highest number of orders followed by Ceaser Salad , Griled Chicken , Pancakes and Oatmeals. From this we can conlude that increaseing the price of these 5 most selling dishes can profit the business.

4. Relationship between Total Orders and Location using bar graph

![image](https://github.com/user-attachments/assets/d3e39950-108d-4240-bf9f-1a3bd0bc47b4)

From the above graph it is obsereved that Chicago has the highest number of orders followed by Boston which indicates that these two states contribute more profit to the company. It may be due to better selling strategy , customer satisfaction, quality of food , which might be compromised in states with lower sales like Austin and Miami. Thee factors could be worked on to improve the profit of the company.

# References
https://pandas.pydata.org/docs/
https://matplotlib.org/stable/index.html
https://seaborn.pydata.org/

