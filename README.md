# matplotlib-challenge
Pymaceuticals

This repository contains a data visualiztion practice of animal study through application of Python Matplotlib. Practice of statistical methods as well as various types of plots are included in the Jupyter Notebook file-pymaceuticals_1.ipynb.

Table Content
1. Background
2. Prepare the Data
3. Generate Summary Statistics
4. Create Bar Charts and Pie Charts
5. Calculate Quartiles, Find Outliers
6. Create a Box Plot
7. Create a Line Plot and a Scatter Plot
8. Calculate Correlation and Regression

1. Background
A new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

Data analysis should be done based on the complete data from the most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The task is to generate all of the tables and figures needed for the technical report of the clinical study. Also, a top-level summary of the study results is required.

2. Prepare the Data
A.	Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.
B. Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.
C. Display the updated number of unique mice IDs.

3. Generate Summary Statistics
Create a DataFrame of summary statistics including:
•	A row for each drug regimen. These regimen names should be contained in the index column.
•	A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

4. Create Bar Charts and Pie Charts
A.	Generate two bar charts. Both charts should be identical and show the total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.
o	Create the first bar chart with the Pandas DataFrame.plot() method.
o	Create the second bar chart with Matplotlib's pyplot methods.
B.	Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.
o	Create the first pie chart with the Pandas DataFrame.plot() method.
o	Create the second pie chart with Matplotlib's pyplot methods.
5. Calculate Quartiles, Find Outliers, and Create a Box Plot
C.	Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:
o	Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
o	Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
o	Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
o	Determine outliers by using the upper and lower bounds, and then print the results.
6. Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

7. Create a Line Plot and a Scatter Plot
A.	Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.
B.	Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

8. Calculate Correlation and Regression
A.	Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.
B.	Plot the linear regression model on top of the previous scatter plot.


