# SF Crime Data Analysis Project

## Overview
This project provides an analysis of crime data in San Francisco from 2003 to 2018. The analysis explores crime trends over time, crime distribution across different districts, and uses predictive modeling to forecast future crime patterns.

The key analyses performed in this project include:

**Time Series Analysis**: A SARIMA model was used to forecast crime trends based on historical data, allowing for predictions of future crime occurrences. This includes training on past data and evaluating performance on test data.

**Exploratory Data Analysis**: Visualizations such as time series plots for monthly and hourly crime data, bar charts for crime categories and districts, and an interactive map displaying incident density across San Francisco.

**Crime Distribution Analysis**: Exploration of crime trends by different categories, times of day, and geographical distribution using statistical visualizations and an interactive Tableau dashboard.

The predictive modeling and visualizations aim to provide a deeper understanding of how crime evolves over time and across different districts of San Francisco, helping in decision-making and public safety strategies.


## Table of Contents
1. [Data](#data)
2. [Data Fields](#data-fields)
3. [Dashboard Visualizations](#dashboard-visualizations)
4. [Tools and Technologies](#tools-and-technologies)
5. [Tableau Dashboard](#tableau-dashboard)
6. [How to Use](#how-to-use)
7. [Findings and Conclusions](#findings-and-conclusions)


## Data
The data used in this analysis was sourced from the San Francisco government’s open data portal and covers a wide range of crime categories across the city from 2003 to 2018.

[Download CSV file](https://drive.google.com/file/d/1YwQnCw3SaheOMSks6TZU_dM6Vrz4tyRI/view?usp=sharing)


### Data Fields:
- **Incident Date**: The date when the crime occurred.
- **Category**: The type of crime committed (e.g., Assault, Larceny, etc.).
- **District**: The district where the crime occurred.
- **Resolution**: The outcome of the crime report (e.g., Arrest, Investigation, etc.).
- **Location**: Geographic coordinates of where the crime occurred.


## Dashboard Visualizations
The following key insights are visualized in the Tableau dashboard:
- **Monthly Crime Data**: A time series plot showing the crime trends by month from 2003 to 2018.
- **Hourly Crime Data**: A line graph showing the distribution of crimes during different hours of the day.
- **Crime Categories**: A bar chart showing the number of crimes per category.
- **District Analysis**: A bar chart showing the number of crimes in each district.
- **Incident Density Map**: An interactive map displaying the density of incidents across different areas in San Francisco.


## Tools and Technologies
- **Tableau Public**: Used for creating interactive visualizations and dashboards to explore and communicate crime data trends.
- **PySpark**: Used for distributed data processing. PySpark’s SparkSession, Row, and SQL libraries were utilized to handle large datasets and perform efficient querying.
- **Pandas**: For data manipulation and cleaning. Used for handling structured data in DataFrames.
- **NumPy**: For numerical computations and efficient array processing.
- **Seaborn**: Used for creating aesthetic and informative statistical visualizations to further analyze trends in the data.
- **Matplotlib**: Used alongside Seaborn for custom visualizations and plot modifications.
- **Python**: The core programming language used for data processing, cleaning, and visualization.
- **Operating System Environment Configuration**: PySpark is configured to run with Python 3 by setting environment variables like PYSPARK_PYTHON.


## Tableau Dashboard
The interactive dashboard for this analysis is available on Tableau Public. You can explore the data and visualizations through the following link:
<a href="https://public.tableau.com/shared/SYST3QZSR?:display_count=n&:origin=viz_share_link" target="_blank">SF Crime Dashboard</a>


## How to Use
1. Click the link above to view the interactive Tableau dashboard.
2. Use the filters explore the data by year, category, district, and resolution.
3. Hover over the data points to view detailed information.


## Findings and Conclusions
**Crime Trends**: The analysis of San Francisco crime data from 2003 to 2018 reveals that theft-related incidents are the most prevalent, followed by other criminal offenses and non-criminal issues. Crime rates tend to peak around 12 PM and 6 PM, indicating key times for heightened law enforcement presence.

**Geographic Hotspots**: The districts of Southern, Mission, and Northern were identified as having the highest concentration of criminal activity. This spatial analysis provides valuable insights into where policing efforts could be focused for maximum impact.

**Unresolved Cases**: Approximately 73.6% of criminal cases remain unresolved, which highlights the need for comprehensive measures aimed at improving investigative outcomes. These findings suggest the necessity of strategic reforms in resource allocation, police training, and community engagement to enhance public safety and justice effectiveness.

**Time Series Forecasting**: A SARIMA model was developed to forecast future crime trends using historical data from 2003 to 2017. The model demonstrated solid predictive capabilities with a mean squared error (MSE) of 162.42, effectively capturing crime patterns and enabling better planning for crime prevention initiatives.
