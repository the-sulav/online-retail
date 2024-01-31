Online Retail Dataset Analysis
This repository contains Python code for analyzing the "Online Retail" dataset obtained from UCI's data repository. The dataset was provided by Dr. Daqing Chen, Director of the Public Analytics group at the School of Engineering, London South Bank University.

Data Source
Source: UCI - Online Retail Dataset
Source Author: Dr. Daqing Chen, chend '@' lsbu.ac.uk, School of Engineering, London South Bank University, London SE1 0AA, UK.
Data Preprocessing
Duplicate Check: Checked and confirmed no duplicate rows in the dataset.

Mapping Check: Explored the mapping between StockCode and Description and found that there are 1324 instances where a StockCode has more than one value for Description. Due to mislabeling or missing values, it is assumed that there is a direct one-to-one mapping between StockCode and Description. Therefore, the Description column is removed from the dataset.

Handling Missing Values:

CustomerID: Filled missing values with "9999" to represent unlabeled customers.
Description: Removed from the dataset.
Feature Engineering:

Introduced a new feature Total_sale_price calculated as the product of Quantity and UnitPrice.
Exploratory Data Analysis (EDA)
Aggregated Quantity by Stock Code:

Visualized the aggregated quantity by StockCode using a bar chart.
Date and Time Separation:

Separated InvoiceDate into Date and Time columns.
Total Sales Analysis:

Explored total sales per year using a pie chart.
Analyzed total sales per month across all time using a bar chart.
Top Customer Analysis:

Identified and excluded the highest spender (CustomerID 9999) from the top 20 highest spenders.
Visualized the top 20 highest spenders using a horizontal bar chart.
Top Items Sold Analysis:

Explored the top N items sold using a bar plot.
Conclusion
The code provides a comprehensive analysis of the "Online Retail" dataset, covering data preprocessing, feature engineering, and exploratory data analysis. The results can be used to gain insights into sales trends, customer behavior, and top-performing items.
