# Road Accident Data - Analysis

Analyzing road accident data in Excel can help you identify trends, hotspots, and potential areas for safety improvements. Here’s a detailed step-by-step guide to analyze such data:
### 1. Data Import and Preparation
	1. Import Data: Load your road accident data into Excel. You can do this by opening the CSV file directly in Excel or using the Data tab to import from various sources.
	2. Data Cleaning: Ensure your data is clean. This involves checking for and handling any missing values, duplicates, and incorrect entries. Use Filter, Conditional Formatting, and Data Validation tools for this.
	3. Data Structuring: Structure your data into meaningful columns, such as:
		○ Date and time of the accident
		○ Location (latitude and longitude or street names)
		○ Type of accident
		○ Number of vehicles involved
		○ Weather conditions
		○ Severity of injuries
### 2. Basic Analysis
	1. Summary Statistics: Use Descriptive Statistics from the Data Analysis Toolpak to get an overview of your data (mean, median, mode, standard deviation, etc.).
	2. Pivot Tables: Create pivot tables to summarize your data. For example, you can group accidents by month, day of the week, or hour of the day to identify trends.
	3. Count and Frequency Analysis: Count the number of accidents by type, location, or weather condition to identify the most common factors involved in accidents.
### 3. Visualization
	1. Bar Charts and Histograms: Use bar charts to compare the number of accidents by category (e.g., type of accident or weather condition). Histograms are useful for visualizing the distribution of numeric data (e.g., number of accidents per hour).
	2. Line Graphs: Plot line graphs to show trends over time, such as the number of accidents per month.
	3. Heat Maps: Create heat maps to visualize accident hotspots. You can do this using conditional formatting or by plotting geographic data on a map (e.g., using Excel’s built-in map charts).
### 4. Advanced Analysis
	1. Correlation Analysis: Use correlation functions (CORREL) to find relationships between different variables (e.g., weather conditions and accident severity).
	2. Regression Analysis: Perform regression analysis to predict the number of accidents based on different factors. You can use the Regression tool from the Data Analysis Toolpak.
	3. Geospatial Analysis: If your data includes geographic coordinates, consider using Power BI or other GIS tools for more advanced spatial analysis.
### 5. Reporting and Insights
	1. Dashboard Creation: Build an interactive dashboard to display your key findings. Use Slicers and Interactive Charts to make it user-friendly.
	2. Summary Report: Create a summary report highlighting the key insights from your analysis. This can include textual descriptions, charts, and tables.
	3. Recommendations: Based on your analysis, provide recommendations for improving road safety. This could include changes in infrastructure, public awareness campaigns, or specific interventions at accident hotspots.
 
* Analyzing road accident data can provide valuable insights into the factors contributing to accidents and help in making data-driven decisions to improve road safety. If you have specific data or need help with a particular analysis, feel free to share more details! *


The raw data was in .csv format. We converted it to .xlsx format for two reaons 
	1. xlsx format has better compression than csv thus smaller file size and 
	2. Support for a table structure as in excel table Format.
	[01_First_Data_View.png]
	
Add two columns 'Month' and 'Year' for which we will extract values from the 'Accident date' column
using =TEXT([@[Accident Date]],"mmm") and =TEXT([@[Accident Date]],"yyyy") formula
convert the two column to 'values' only.
[02_ColumnsAdded.PNG]

Import the excel table into a new excel file>Get Data>From file>From excel workbook
[03_ImportData.PNG]
select the table we created in earlier step and in import data dialog select "only create connection"
[04_connOnly.PNG]

Add three worksheets for Analysis
1. Road Type - for road cndition analysis
2. Monthly Trend - Monthly accident trends
3. KPI - Key parameters


1. Road Type - for road cndition analysis
	We need to create few pivot tables and charts analysing road condition at the time of accident
	a. Number of casualties by road type
	b. 
	
	
	
	'[Road Accident Data.csv]Road Accident Data'!$A$1:$W$307974



	
	