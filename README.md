
THREE OBSERVATIONS:


1. In the summary statistics comparing Capomulin to every other drug regimen. The only other drug that comes close in mean, median, variance, std, sem is the Ramicane drug. They are both at the lowest tumor volume for each statistics. 

2. After viewing the result of the pie chart, the distribution of sex between the mice are about even for female and male testing. 

3. The correlation coefficient between mouse weight and average tumor volume for the Capomulin regimen is 0.84, displaying a strong and significant positive correlation.


---------------------------------------------------------------------------------------------------------------------------------------------------------------------
INSTRUCTIONS


Prepare the Data


1.Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

2.Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

3.Display the updated number of unique mice IDs.

Create two summary statistics DataFrames:

For the first DataFrame, use the groupby method to generate the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen. This should result in five unique Series objects. Combine these objects into a single summary statistics DataFrame.

For the second DataFrame, use the agg method to produce the same summary statistics table by using a single line of code.

GENERATE BAR CHARTS & PIE CHARTS
1.Generate two bar charts. Both charts should be identical and show the total number of time points for all mice tested for each drug regimen throughout the study.

Create the first bar chart with the Pandas DataFrame.plot() method.

Create the second bar chart with Matplotlib's pyplot methods.

2.Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

Create the first pie chart with the Pandas DataFrame.plot() method.

Create the second pie chart with Matplotlib's pyplot methods.

Calculate Quartiles, Find Outliers, and Create a Box Plot

1.Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

  Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

  Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

  Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment.
  Append the resulting final tumor volumes for each drug to the empty list.

  Determine outliers by using the upper and lower bounds, and then print the results.

2.Using Matplotlib, generate a box plot of the final tumor volume for all four treatment regimens. Highlight any potential outliers in the plot by changing their color and style.

Create a Line Plot and a Scatter Plot


1.Select a mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

2.Generate a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.

Calculate Correlation and Regression


1.Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.

2.Plot the linear regression model on top of the previous scatter plot.
