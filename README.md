# CIS_410_Assignment3_Fall2024
Write a brief description of the results and include that int he body of the README.md file.

In JupyterLab, I read the data from the avocado.csv file into a DataFrame in order to analyze the data. 
I used the info() method to see the data type, memory comsuption,and null count information and the results showed that there are 9 float64, 2 int64, and 3 object data types, a memory usage of 1.9+ MB, and that all are non-null.
The nunique() function I used to see the number of unique values in each column results; 
Unnamed: 0         53
Date              169
AveragePrice      259
Total Volume    18237
4046            17702
4225            18103
4770            12071
Total Bags      18097
Small Bags      17321
Large Bags      15082
XLarge Bags      5588
type                2
year                4
region             54
dtype: int64

The first and last five rows are listed from 0-4, and 18244-18248
The last four columns of data are listed as XLarge Bags, type, year, and region

I used data[['Date','AveragePrice','Total Volume']].head() to display the first 5 rows of data only showing the Date, AveragePrice, and Total Volume and data.AveragePrice to display the average price for the first and last five rows.

I created a new column called EstimatedRevenue by multiplying the Total Volume by the AveragePrice in each row and only displayed the first five rows.
I created a new DataFrame and grouped it by type and region while including the AveragePrice as well.

With the groupby DataFrame, I created a bar plot to show the mean, median, and standard deviation of the Total Volumn by year. The data seems to have slight changes by year with the std. mean, and median for year 2018 being the highest.

I created a new DataFrame that includes all the bag sizes grouped by type (convential and organic).
With that data, I created a bar plot that shows the total number of bags by type with the results showing higher numbers for the convential type.

I created a scatter plot with the original data using Total Volume in the x asis and AveragePrice in the y asis. 


