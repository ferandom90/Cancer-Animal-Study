# Cancel Animal Study

Analysis
This code imports necessary libraries and reads from two csv files containing data on mice and the results of a drug study. It then merges the two datasets into one based on their shared Mouse ID.
Next, it checks for duplicate mice in the dataset and removes them to create a clean dataset.
It then calculates summary statistics (mean, median, variance, standard deviation, and SEM) for the tumor volume of each drug regimen and creates two tables summarizing this information: summary_table and summary.
Two bar plots are generated, one using Pandas and the other using pyplot, showing the total number of mouse timepoints for each drug regimen. We can observe that (Capomilun and Ramicane) have the most timepoints both over 200 each, compare to (Propriva) that was the lowest parametres. Two pie charts are also created showing the distribution of female versus male mice (51% v 49%), showing that male has a slightly more percetage over females, one using Pandas and the other using pyplot.
Next, we calculate the final tumor volume of each mouse across four specific treatment regimens (Capomulin, Ramicane, Infubinol, and Ceftamin) and creates a box plot showing the distribution of final tumor volumes for each treatment. Infubinal is noteworthy in this box plot as it has an outlier outside of the upper and lower bands at 36.321346 and this is highlights with a circle colored in red.
Next, we created line plots and the first plot shows the relationship between tumor volume and time point for a single mouse treated with Capomulin. The x-axis represents the time point (in days), and the y-axis represents the tumor volume (in mm3). The plot helps visualize how the tumor volume changes over time in response to the treatment. You can see that Timepoint 20 days, the tumor volume is 48 mm3 and begins to drop significantly in the following timepoints.
The second plot is a scatter plot that shows the relationship between mouse weight and the average observed tumor volume for the entire Capomulin regimen. The x-axis represents the weight of the mouse (in grams), and the y-axis represents the average tumor volume (in mm3). The plot helps visualize any potential correlation between mouse weight and tumor volume, as heavier mice may be expected to have larger tumors.
Finally, we calculate the correlation coefficient = .84, a strong positive correlation. Then we calculate a linear regression model for mouse weight and average observed tumor volume for the entire Capomulin regimen. The correlation coefficient measures the strength and direction of the linear relationship between the two variables. The linear regression model helps quantify the relationship between the variables and predict the value of the dependent variable (tumor volume) based on the independent variable (mouse weight).
Linear Regression Results:
slope = 0.9544396890241048 intercept = 21.552160532685008 rvalue = 0.8419363424694721 pvalue = 1.3225722434712404e-07 stderr = 0.12754359033201323 intercept_stderr = 2.5909876867683455
The code then generates a scatter plot of the data and overlays a line that represents the linear regression model. The plot also displays the correlation coefficient and a title that summarizes the findings of the analysis.

