
# Road Accident Data - Analysis
# ___From accidents to action: insights that save___


### _This project envisions safer roads through data‑driven insights — predicting accident trends, identifying high‑risk scenarios, and guiding proactive interventions that reduce casualties and improve public safety._





## Data Import and Preparation</p>


- Import Data: Load your road accident data into Excel. You can do this by opening the CSV file directly in Excel or using the Data tab to import from various sources.
- Data Cleaning: Ensure your data is clean. This involves checking for and handling any missing values, duplicates, and incorrect entries. Use Filter, Conditional Formatting, and Data Validation tools for this.
- Data Structuring: Structure your data into meaningful columns, such as:
    * Date and time of the accident
    * Location (latitude and longitude or street names)
    * Type of accident
    * Number of vehicles involved 
    * Weather conditions
    * Severity of injuries

---

##  Basic Analysis</p>

- Summary Statistics: Use Descriptive Statistics from the Data Analysis Toolpak to get an overview of your data (mean, median, mode, standard deviation, etc.).
- Pivot Tables: Create pivot tables to summarize your data. For example, you can group accidents by month, day of the week, or hour of the day to identify trends.
- Count and Frequency Analysis: Count the number of accidents by type, location, or weather condition to identify the most common factors involved in accidents.

---

## Visualization</p>

- Bar Charts and Histograms: Use bar charts to compare the number of accidents by category (e.g., type of accident or weather condition). Histograms are useful for visualizing the distribution of numeric data (e.g., number of accidents per hour).
- Line Graphs: Plot line graphs to show trends over time, such as the number of accidents per month.
- Heat Maps: Create heat maps to visualize accident hotspots. You can do this using conditional formatting or by plotting geographic data on a map (e.g., using Excel’s built-in map charts).

---

## Advanced Analysis</p>

- Correlation Analysis: Use correlation functions (CORREL) to find relationships between different variables (e.g., weather conditions and accident severity).
- Regression Analysis: Perform regression analysis to predict the number of accidents based on different factors. You can use the Regression tool from the Data Analysis Toolpak.
- Geospatial Analysis: If your data includes geographic coordinates, consider using Power BI or other GIS tools for more advanced spatial analysis.

---

## Reporting and Insights </p>

- Dashboard Creation: Build an interactive dashboard to display your key findings. Use Slicers and Interactive Charts to make it user-friendly.
- Summary Report: Create a summary report highlighting the key insights from your analysis. This can include textual descriptions, charts, and tables.
- Recommendations: Based on your analysis, provide recommendations for improving road safety. This could include changes in infrastructure, public awareness campaigns, or specific interventions at accident hotspots.

---

* Analyzing road accident data can provide valuable insights into the factors contributing to accidents and help in making data-driven decisions to improve road safety. If you have specific data or need help with a particular analysis, feel free to share more details! *

---

#### Note on .csv and .xlsx - Excel format has advantage over csv format in that it supports table structure, and multiple sheets in one file. Though data is mostly exported/received in csv format as this being a universal format. For our analysis we will save the data in 
---

# Cleaning the data </p>

### For cleaning purpose following steos are taken
* key column validation such as 'Accident index', and other dimensional columns such as 'Accident_Severity','Vehicle_Type' etc.
* Checking for Inconsistencies, typo error, spellings and invalid data.
* Blank columns and data not available.

### Data Processing
* Add columns 'Month' with formula =TEXT([@[Accident Date]],"mmm"). convert to values only.
* Add columns 'Year' with formula =TEXT([@[Accident Date]],"yyyy"). convert to values only.

</p>



![02_ColumnsAdded.PNG](https://github.com/tejashazaree/Road-Accident---Data-Analysis---Excel/blob/main/Images/02_ColumnsAdded.PNG)


> with the Cleaning and Processing part done our data is ready for Analysis.

### Data Analysis and Visualization

Add four worksheets for Analysis
1. Road Type - for road condition analysis.
2. Monthly Trend - Monthly accident trends.
3. KPI - Key parameters.
4. Data Analysis.


#### Import the excel table into a new excel file>Get Data>From file>From excel workbook
![03_ImportData.PNG](https://github.com/tejashazaree/Road-Accident---Data-Analysis---Excel/blob/main/Images/03_ImportData.PNG)

#### In the Import Data dialogue check 'Only Create Connection' as data file is separate from the Dashboard file.

![03_ImportData.PNG](https://github.com/tejashazaree/Road-Accident---Data-Analysis---Excel/blob/main/Images/04_connOnly.PNG)

---

#### Add a sheet rename it to 'KPI' and add all the required pivot tables and charts as per below image. Use 'From external data source' to create pivot tables. 

![06_KPI-Sheet.PNG](https://github.com/tejashazaree/Road-Accident---Data-Analysis---Excel/blob/main/Images/06_KPI-Sheet.png)

---

#### Add a monthly trends pivot table in 'Monthly Trends' sheet as show in the image.

![Monthly Trends](https://github.com/tejashazaree/Road-Accident---Data-Analysis---Excel/blob/main/Images/07_Mnthly-Trends.png)

---

#### Add pivot table for Road type analysis and charts.

![Road Type](https://github.com/tejashazaree/Road-Accident---Data-Analysis---Excel/blob/main/Images/08_Road-Type.png)

---
### The Dashboard

#### We need to consolidate all the analysis on a single page usually a screen size. All the summary chart and controls are added. Filters based on year and area wise are useful.

![05_Dashboard.PNG](https://github.com/tejashazaree/Road-Accident---Data-Analysis---Excel/blob/main/Images/05_Dashboard.png)

---
# Descriptive Analytics - Telling the story of what happened

>Here’s a summary you of the Road Accident data:
>- Total casualties: 417,883 across 2021–2022, with a 12% drop in >2022 compared to 2021.
>- Severity breakdown: Slight injuries dominate (≈84%), serious >injuries (≈14%), and fatalities are relatively low (≈2%).
>- Vehicle involvement: Cars are the major contributor (≈80% of >casualties), followed by bikes and vans.
>- Road type: Single carriageways account for nearly >three-fourths of all casualties, making them the riskiest.
>- Conditions: Most accidents occur on dry roads (≈67%), in urban >areas (≈61%), and during daylight (≈73%).
>- Monthly trend: Casualties peak in October–November and dip in >February–December, showing seasonal variation.

👉 In short: Urban, daylight accidents on single carriageways involving cars are the biggest risk factors, though overall casualties are declining year-on-year.

---

# Diagnostic Analysis - Uncovering why accidents occur
>- Target high‑risk zones: Focus safety interventions on single >carriageways in urban areas, where the majority of casualties >occur.
>- Vehicle‑specific measures: Prioritize awareness and >enforcement for car drivers, since they account for ~80% of >casualties.
>- Behavioral campaigns: Address congestion‑related minor >collisions through speed management, distraction reduction, and >safe‑driving education.
>- Seasonal preparedness: Implement extra safety checks and >campaigns during October–November, when accident peaks are >observed.
>- Infrastructure improvements: Enhance road design, signage, and >lighting on single carriageways to reduce exposure to high‑risk >conditions.

---

# Predictive Analysis - Forecasting tomorrow’s road risks today

>- Casualty Trend Forecast:
>With a 12% decline from 2021 to 2022, if similar improvements continue, total >casualties could drop to around 170K–175K annually by 2023–2024.
>- Severity Outlook:
>Fatalities are consistently under 2% of total cases. This proportion is likely >to remain stable, while slight injuries will continue to dominate (>80%), >reflecting congestion-driven minor collisions.
>- High-Risk Scenarios:
>- Cars on single carriageways in urban daylight will remain the primary risk >combination.
>- Unless infrastructure changes are made, single carriageways will continue to >account for ~70–75% of casualties.
>- Seasonal Predictions:
>Accident peaks in October–November are expected to persist due to holiday >traffic surges. Preventive campaigns during these months could significantly >reduce casualties.
>- Impact of Road Conditions:
>Dry road accidents will remain dominant (>65%), suggesting that traffic density >and driver behavior will continue to outweigh weather as a predictive factor.


---

# Prescriptive Analysis - Guiding safer roads with smart actions

>- Upgrade Roads: Improve single carriageways in urban areas with dividers, lane >markings, and better lighting.
>- Enforce Behavior: Strengthen speed limit enforcement, seatbelt checks, and >distracted driving laws for car drivers.
>- Seasonal Campaigns: Launch targeted safety drives in October–November to >reduce predictable accident spikes.
>- Educate Drivers: Promote safe driving practices (lane discipline, following >distance, reduced speeding in congestion).
>- Adopt Technology: Deploy collision-avoidance systems, CCTV monitoring, and >smart traffic signals in high-risk zones.
>- Data-Driven Policing: Use accident trend data to allocate resources and >patrols to hotspots for maximum impact.



---

##### If you would like to create the dashboard there is a tutorial available on Youtube.

https://www.youtube.com/watch?v=XeWfLNe3moM