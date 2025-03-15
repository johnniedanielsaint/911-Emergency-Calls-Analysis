:

📌 Project Objective:
Analyze the 911 calls to uncover insights such as:

The most common reasons for 911 calls.
Distribution of calls by township and ZIP code.
Call trends over time (daily, monthly, yearly).
Comparison of call types (Traffic, EMS, Fire).
Geographical distribution of calls.
🔍 Steps to Build the Power BI Project:
Load Data into Power BI:

Open Power BI Desktop.
Click on "Get Data" > "Text/CSV" and load the 911.csv file.
Data Transformation (Power Query):

Remove unnecessary columns if needed (e.g., e column if it's not useful).
Split the title column to extract the Reason:
Go to Transform Data > Split Column > By Delimiter (:) > Choose the first occurrence.
Rename the new column as Reason.
Change data types where appropriate (e.g., 'timeStamp' to Date/Time format).
Creating Measures and Calculations:

Create new columns where necessary:
Extract Hour, Month, Day of Week from the 'timeStamp' column.
Create calculated columns for better analysis:

Hour = HOUR([timeStamp])
Month = MONTH([timeStamp])
DayOfWeek = FORMAT([timeStamp], "dddd")
Building Visualizations:

Bar Chart: Number of Calls by Reason.
Map Visualization: Calls by ZIP code and Township (twp).
Line Chart: Number of Calls over Time (Daily/Monthly Trends).
Heatmap: Calls by Hour of Day vs. Day of the Week.
Pie Chart: Proportion of Calls by Reason (Traffic, EMS, Fire).
Adding Filters and Slicers:

Add Date Range Filters.
Add Slicers for Reason, Township, ZIP Code.
Dashboard Design:

Create a clean and professional layout with visuals arranged by theme.
Add titles, tooltips, and descriptions for clarity.


