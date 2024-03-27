Sales Analysis Project for Data Analytics Certification - 
Project Statement

AAL, a prominent Australian clothing brand since 2000, is expanding its business and needs assistance from the Head of Sales and Marketing (S&M) to make informed investment decisions. The tasks include identifying high-revenue states and creating sales programs for low-revenue states. Analyze the company's Q4 sales data in Australia, state by state, to provide data-driven insights for decision-making in the next year.

Steps:
1 - Evaluate the Data Set
1B. Handling Null Values - none in data set, but below are options for what to do with null values when presented with them in a data set.
Option A: use the 'dropna()' method to remove rows conatining null values: df.dropna(inplace=True)
Option B: use the 'fillna()' method, such as filling nulls with the mean of the column: df.fillna(df.mean(), inplace=True)
Option C: use forward fill or backward fill to fill the nulls with the previous or next non-null value: df.ffill(inplace=True)
df.bfill(inplace=True)
Option D: Interpolate missing values based on the existing values in the dataset: df.interpolate(inplace=True)

1C. Choose a Data Wrangling Technique

In order to do so you want to understand your data, which you can call using and df.info. Based on the data and goals of AAL, the recommended normalization technique is Min-Max scaling and apply it to the 'Sales' column, to see which states have the highest revenue and which states have the lowest, since this is one of their main goals. 

1D. Share insights regarding GroupBy() Function

Once you have more information about the data set, compare that to what the companies goals are. Based off of their goal to identify the states with the highest revenues and develop sales programs for states with lower revenues, it makes sense to group the data by states and sales first to identify who has the highest and who has the lowest.
Based on this data, the state with the highest sales is Victoria, with a high variability indicating that the total sales values for Victoria are considerably spread out from the mean. The state with the lowest sales is Western Australia, with a moderate variability, indicating that the total sales values have some spread from the mean.
Given that the mean, median, and mode are relatively similar for each state, the distribution of the total sales is going to be relatively symmetric/normal for all of them, and also further confirms the lack of outliers skewing the data.

1D cont.
Since we are only examining the 4th quarter, you can also use the groupby() and datetime functions to group the sales by month, and then proceed to compare it to multiple columns from there.
Based on what the data is showing after breaking it down further, you can see the highest sales month is December with October as a close second. You can deduce that given the holiday season, end of school year, high vacation and travel times, and seasonal change that it makes sense these would be times of the year with higher sales. Then when broken down by group and state, you can see men in Victoria had the highest sales during that time, followed closely by seniors and women in Victoria, which is likely because parents and grandparents are buying presents for their kids and loved ones. 

You can also see Western Australia and Northern Territory have the lowest sales in November, which further adds credibility to the other insights. It would make sense to research the populations, number of stores, and cultural holidays in those territories to get further insights as to what the training could look like to improve sales. 

2 -  Data Analysis 
2A. Perform descriptive statistical analysis on 'Sales' and 'Unit' columns
2B. Determine which group is generating the highest sales and which group is generating the lowest sales.
2C. Determine which state is generating the highest sales, and which state is generating the lowest sales.
2D. Generate weekly, monthly, and quarterly reports for the analysis made.

 3 - Data Visualization
 3A. Using seaborn and matplotlib, create charts making visuals for your previous recommendations and analyses.
 

