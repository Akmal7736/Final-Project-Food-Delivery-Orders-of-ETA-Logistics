

Food Delivery Orders 
Of
 ETA Logistics


AKMAL
DA55




INDEX
        Content                                  Page

•	Summary                                                                            1
•	Introduction                                                                      2 
•	Project Objective                                                              3
•	Dataset Description                                                         4
•	Using Tools & Libraries and Data Loading               5
•	Data Cleaning                                                                   6
•	Data Visualization                                                        7-9
•	Findings and Insights                                                              10








Summary

This project analyzes the food delivery orders dataset for ETA Logistics, which includes detailed information about orders, customers, restaurants, and drivers. The analysis primarily aims to uncover key insights regarding delivery times, peak operating hours, busiest days, customer segmentation, and overall restaurant performance.
The project further involves conducting Exploratory Data Analysis on real-world delivery data, including data cleaning and anomaly handling such as missing-value imputation, duplicate verification, and zero-value treatment. It uses Matplotlib and Seaborn to visualize data, generate market insights, and formulate strategic recommendations.















Introduction

In the fast paced modern food service industry, efficient logistics and timely delivery are critical to ensuring customer satisfaction. Also this industry is comparatively very competitive. So this project focuses on analyzing the food delivery order dataset for ETA Logistics to find valuable operational insights. 

By examining various factors such as restaurant delivery time, customer rating and behavior, orders in different categories, customers' payment methods, checking invalid values, finding correlations, observing charges, and peak operating hours and days, this study identifies a clear pattern. 

Using Exploratory Data Analysis including data cleaning and handling. For better understanding helps data visualization using matplotlib ,seaborn and plotly. This reports provides finding to help optimize  proper logistics operations. It ensures improvement in delivery efficiency and enhances customer satisfaction.










Project Objective

•	This project aims to perform an in-depth Exploratory Data Analysis to uncover actionable insights. 
•	Cleaning the dataset.
•	Identifying peak delivery times.
•	Analyzing customer behavior.
•	Evaluating restaurant performance to minimize delivery latency.












Dataset Description

This dataset contains 49,132 rows and 36 columns. Providing detailed information on orders, customers, restaurants, and deliveries. Sourced from Kaggle, it covers various aspects of the delivery process. The columns contain numerical data, dates and objective data.



















Using Tools and Libraries

Data cleaning:-
•	Pandas
•	Numpy

Libraries:-
•	Matplotlib
•	Seaborn
•	Plotly

Data Loading

To load the dataset, first import the Pandas library. The dataset is in an Excel file, so use the read function to load the dataset from the specified file path into a variable named “Data”. Then create a data frame named “df”.







Data Cleaning
These are the steps used for data cleaning..
•	Duplicate Check: Checked the dataset for duplicate values using df.duplicated().sum().

•	Null Value Imputation: Identified missing and resolved them by filling customer_age and restaurant_rating with mean values, and customer_type, restaurant_primary_category and restaurant_type columns with mode values.

•	Dropping Rows: Removed 868 rows representing cancelled orders from the dataset.

•	Data Type Correction: Checked column data types and corrected incorrect ones (such as changing customer_age from float to int).

•	Data consistency check: Checked data consistency in columns

•	Outlier Check: Checked for outliers in the dataset using the IQR (Interquartile Range) method.







Data Visualization

A total of 6 plots were used for visualization..
•	The Bar Plot: illustrates the distribution of orders across various restaurant types.
Orders are concentrated in different categories.
 

•	The Pie Chart: Analyzes the different payment methods used by customers. Most customers are likely to order food using a credit card 
•	The Box Plot: The box plot reveals numerous outliers for order totals and it shows outliers, with many orders significantly above the median, indicating the presence of exceptionally large orders in the dataset.
 

•	The Heatmap: Explores the correlation between different variables in the dataset. It shows a strong positive correlation between restaurant preparation time and order total and it meaning that larger orders take longer to prepare. It also shows a positive correlation between estimated delivery time and actual delivery time. This correlation means orders are delivered on time.
 
•	The Violin Plot: It shows the distribution, density, and spread of ratings across four distinct restaurant categories: Casual Dining, Cafe, Fast Food, and Fine Dining. By combining a box plot with a kernel density estimation, it highlights both the central tendency (medians and quartiles) and the frequency of specific rating values for each category. 
•	The Line Chart: Depicts the hourly trends of orders throughout the day. This graph shows the distribution of hourly orders. Orders start increasing around 5 AM and the peak time is around 11 AM; then orders go higher again, peaking around 7 PM.
 
Findings and Insights
•	The analysis reveals several key patterns in food delivery operations. 
•	Fine dining restaurants generate the highest order volume, whereas cafes process the fewest orders.
•	Regarding delivery efficiency, fast food establishments offer the quickest turnaround times, while fine dining orders require the longest preparation and transit periods.
•	In terms of consumer preferences, burgers are the most ordered item category
•	The majority of customers pay using credit cards and digital wallet transactions compared to cash.
•	Order activity shows distinct daily peaks (starting around 5 AM, peaking during lunch hours around 11 AM–1 PM, and another peak during evening dinner hours around 7 PM–9 PM).
•	A strong positive correlation exists between restaurant preparation time, actual delivery time, and distance.
•	Delivery rider allocation and restaurant operations should be dynamically scaled up during peak lunch and dinner windows to manage surge demand effectively.
