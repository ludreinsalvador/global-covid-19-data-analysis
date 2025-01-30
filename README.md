# The-Global-Covid-19_Cases-Deaths-and-Vaccination-Trends

## About the Project
This project focuses on creating an interactive PowerBI dashboards to visualize and analyze global COVID-19 data sourced from the World Health Organization (WHO). The dashboards offers insights into the spread, impact, and vaccination progress of COVID-19 across various regions.

## Objectives/Problems
- To provide a clear visual representation of COVID-19 cases, deaths, and vaccination rates globally.
- To identify trends and patterns in the data that can inform public health decisions.
- To offer an interactive tool for users to explore COVID-19 data at various granularities (e.g., by country, region, and over time).

## Dataset Used
The dataset, sourced from the World Health Organization (WHO), provides authoritative global data on COVID-19 cases, deaths, and vaccinations. It is crucial for analyzing the pandemic's impact and monitoring vaccination progress worldwide.
- <a href="https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/WHO-COVID-19-global-data.csv">WHO-COVID-19-global-data.csv</a> - Contains daily reports on COVID-19 cases and deaths for various countries and regions.
- <a href="https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/vaccination-data.csv">vaccination-data.csv</a> - Contains data on COVID-19 vaccinations, including the number of doses administered and the number of people vaccinated by country.
  
## Questions (KPIs)
- How have COVID-19 cases and deaths evolved globally over time?
- Which countries or regions have the highest number of cases and deaths?
- What are the trends in vaccination rates across different countries?
- How does the number of cases correlate with vaccination rates?
- Are there any noticeable patterns in the data that suggest successful or unsuccessful public health strategies?

## Key Data Columns Include:
- Date: The specific date of the report.
- Country/Region: The name of the country or region.
- New cases: The number of new COVID-19 cases reported on that date.
- Cumulative cases: The total number of COVID-19 cases reported up to that date.
- New deaths: The number of new COVID-19 deaths reported on that date.
- Cumulative deaths: The total number of COVID-19 deaths reported up to that date.
- Total vaccinations: The total number of vaccine doses administered up to that date.
- People vaccinated: The number of individuals who have received at least one dose of a COVID-19 vaccine.
- People fully vaccinated: The number of individuals who have received all required doses of a COVID-19 vaccine.

## Proposed Visualizations
- Global Trends Line Chart:
  - X-axis: Date
  - Y-axis: Number of cases/deaths
  - Series: New cases, New deaths
- Heat Map:
  - Dimensions: Countries/Regions
  - Color Scale: Number of cases/deaths
- Bar Chart:
  - X-axis: Countries/Regions
  - Y-axis: Total vaccinations, People vaccinated, People fully vaccinated
- Scatter Plot:
  - X-axis: Total vaccinations
  - Y-axis: Number of cases
  - Size: Population
- Map Visualization:
  - Dimensions: Geographic locations
  - Color/Size Indicators: Number of cases, Deaths, Vaccination rates

## Process
#### Data Cleaning (WHO-COVID-19)
- Replaced `null` values with `0` for consistency.
- Replaced blank rows with `Other` to maintain data integrity.
- Changed data types from `Decimal Number` to `Whole Number` where needed.

#### Data Cleaning (Vaccination Data)
- Removed irrelevant columns to simplify the dataset.
- Replaced blank rows with `Other` and `null` values with default date or `0` for consistency.

#### Data Transformation
- **Data Types**: Text, Date (from vaccination data), and Number (Decimal or Whole).
- **Transformation Steps**:
  - Split and combined columns for better organization.
  - Merged date columns for both COVID-19 and vaccination data.
  - Appended data and performed calculations for new metrics.
  - Grouped and sorted data for clearer insights (e.g., by country).
  
#### Calculated Columns and Measures
- Created custom calculated columns (`Ambross`, `Luds`) and measures for deeper insights.

#### Model Optimization
- Optimized fact table for faster processing and analysis.

#### Report Enhancements
- Added conditional formatting, slicers, filters, bookmarks, and drillthroughs for interactive and dynamic reporting.

#### Publishing and Workspace Management
- Published the report to Power BI Service.
- Created a Final Exam workspace and app, published reports and dashboards, and shared the app link.

#### Advanced Analytics
- Used features like scatter with animation, clustering, Q&A, Key Influencers, Decomposition Tree, and forecasting for in-depth analysis.

#### Dataset Management
- Managed parameters for flexible and dynamic data exploration.



## Dashboards

