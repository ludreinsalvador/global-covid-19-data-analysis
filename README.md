# The Global Covid-19: Cases, Deaths, and Vaccination Trends

## About the Project
This project focuses on creating interactive Power BI dashboards to visualize and analyze global COVID-19 data sourced from the World Health Organization (WHO). The dashboards offer insights into the spread, impact, and vaccination progress of COVID-19 across various regions.

---
## Objectives
- Provide a clear visual representation of COVID-19 cases, deaths, and vaccination rates globally.
- Identify trends and patterns in the data to inform public health decisions.
- Offer an interactive tool for users to explore COVID-19 data by country, region, and over time.

---
## Dataset Used
Sourced from the World Health Organization (WHO), this dataset provides authoritative global data on COVID-19 cases, deaths, and vaccinations.

- [WHO-COVID-19-global-data.csv](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/WHO-COVID-19-global-data.csv) - Daily reports on COVID-19 cases and deaths per country/region.
- [vaccination-data.csv](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/vaccination-data.csv) - Vaccination data, including doses administered and people vaccinated.

---
## Key Questions
- How have COVID-19 cases and deaths evolved globally over time?
- Which countries/regions have the highest cases and deaths?
- What are the trends in vaccination rates across different countries?
- How does the number of cases correlate with vaccination rates?
- What patterns indicate successful or unsuccessful public health strategies?

---
## Key Data Columns
- **Date**: Specific report date.
- **Country/Region**: Name of the country or region.
- **New Cases**: Daily reported COVID-19 cases.
- **Cumulative Cases**: Total reported cases up to that date.
- **New Deaths**: Daily reported COVID-19 deaths.
- **Cumulative Deaths**: Total reported deaths up to that date.
- **Total Vaccinations**: Total administered vaccine doses.
- **People Vaccinated**: Individuals who received at least one dose.
- **People Fully Vaccinated**: Individuals with all required doses.

---
## Proposed Visualizations
- **Global Trends Line Chart**
  - X-axis: Date | Y-axis: Cases/Deaths | Series: New Cases, New Deaths
- **Heat Map**
  - Dimensions: Countries/Regions | Color Scale: Cases/Deaths
- **Bar Chart**
  - X-axis: Countries/Regions | Y-axis: Vaccinations
- **Scatter Plot**
  - X-axis: Vaccinations | Y-axis: Cases | Size: Population
- **Map Visualization**
  - Location-based cases, deaths, and vaccination rates

---
## Data Storyboard
![Data Storyboard](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/data-storyboard.png)

---
## Data Processing
### Data Cleaning (WHO-COVID-19 Data)
- **Replaced `null` values with `0`** to avoid missing data.
- **Replaced blank rows with `Other`** for consistency.
- **Converted decimal values to whole numbers** where applicable.

### Data Cleaning (Vaccination Data)
- **Removed unnecessary columns** for clarity.
- **Replaced blank rows with `Other`** for consistency.
- **Filled `null` dates with a default value** to prevent errors.
- **Replaced `null` values with `0`** in numerical fields.

### Data Transformation
- **Splitting & Combining Columns**: Normalized and merged relevant fields.
- **Date Merging**: Unified vaccination and COVID-19 data timelines.
- **Appending Data**: Merged datasets from different sources.
- **Calculated Metrics**: New fields like `Vaccination Rate`, `Case Fatality Ratio`.
- **Grouping & Sorting**: Organized data by region, country, and trends.

### Calculated Columns & Measures
- **Calculated Columns**: Custom calculations for deeper insights.
- **Calculated Measures**: Derived measures to quantify COVID-19 trends.

---
## Semantic Modeling
![Semantic Model](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/semantic-model.png)

---
## Model Optimization
- **Optimized fact tables** for faster processing.
- **Applied indexing and efficient relationships** to enhance performance.

---
## Report Enhancements
- **Conditional Formatting**: Highlight key trends.
- **Slicers & Filters**: Enable dynamic data exploration.
- **Bookmarks & Drillthrough**: Improve navigation and depth of analysis.

---
## Advanced Analytics
- **Scatter with Animation**: Showcases trends over time.
- **Clustering**: Identifies patterns among countries/regions.
- **Q&A Functionality**: Interactive querying of data.
- **Key Influencers**: Determines significant data factors.
- **Decomposition Tree**: Breaks down complex data insights.
- **Forecasting**: Predicts COVID-19 trends.
- **Symmetry Shading**: Highlights anomalies.

---
## Dataset Management
- **Parameters**: Allows dynamic data adjustments for better analysis.

---
## Dashboards
- [WHO Global COVID-19 Dashboards (PDF)](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/WHO_global-covid-19_dashboards.pdf)
- [Power BI Dashboard File](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/WHO_global-covid-19_dashboards.pbix)

### Preview of Dashboards:
![Global Covid-19 Overview](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/global-covid-19_overview.png)
![Global Vaccination Analysis](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/global-vaccination_analysis.png)
![2023 Vaccination Rates](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/2023_vaccination-rates.png)
![Global Covid-19 Trends Outcome](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/global-covid-19_trends-outcome.png)
![Global Vaccination Trends Influencers](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/global-vaccination_trends-influencers.png)

---
## Paginated Report
- [COVID-19 Vaccination Report (PDF)](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/WHO_global-covid-19_vaccination-paginated-report.pdf)

