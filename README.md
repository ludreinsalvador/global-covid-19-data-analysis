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
- **Replaced `null` values with `0`**: Ensured missing data for COVID-19 metrics (cases, deaths) is represented as zero, rather than leaving gaps in the dataset.
- **Replaced blank rows with `Other`**: For rows where no data is available, blank spaces were replaced with a generic "Other" category to avoid errors in analysis.
- **Changed data types**:
  - Converted `Decimal Numbers` to `Whole Numbers` where appropriate to match the expected format for certain fields (e.g., case counts, deaths, etc.).

#### Data Cleaning (Vaccination Data)
- **Removed unnecessary columns**: 
  - Columns such as `ISO3`, `DATA_SOURCE`, `DATA_UPDATED`, `TOTAL_VACCINATION_PER_100`, `PERSONS_VACCINATED_1PLUS_DOSE`, and others that did not provide significant insights were removed for clarity and efficiency.
- **Replaced blank rows with `Other`**: Any rows with missing values were categorized as "Other" to maintain consistency and ensure no data was omitted unintentionally.
- **Replaced `null` values with default date**: For missing date fields, a default placeholder date was used to prevent errors in time-based analysis.
- **Replaced `null` values with `0`**: Numerical fields with missing values were filled with `0` to avoid calculation errors during data analysis.

#### Data Transformation
- **Data Types**: 
  - The dataset includes various types of data:
    - **Text** for categorical variables like country names.
    - **Date** (from vaccination data) for tracking timelines and trends.
    - **Number** (Decimal, Whole, or both) for quantitative data (e.g., case counts, vaccination rates).

- **Transformation Methods**:
  - **Splitting columns**: Divided combined columns to normalize data for easier analysis.
  - **Combining columns**: Merged related columns (e.g., merging country and region into one column for broader analysis).
  - **Merging columns**: Merged specific columns like country data with corresponding COVID-19 metrics for better regional analysis.
  - **Date Merging**: Unified date columns from both vaccination and COVID-19 data sources to align time-based insights.
  - **Appending data**: Combined datasets from different sources (e.g., different regions or periods) for a complete analysis.
  - **Calculating new metrics**: Generated new calculated columns (e.g., `Vaccination Rate`, `Case Fatality Ratio`) to aid in deeper insights.
  - **Grouping data**: Aggregated data (e.g., by country or continent) to derive high-level insights or regional comparisons.
  - **Sorting data**: Sorted data (e.g., alphabetically by country) to simplify reporting and highlight specific patterns.

#### Calculated Columns and Measures
- **Calculated Columns**:
  - A custom calculation based on specific data transformations.
  - Another calculated column representing a unique transformation based on the dataset’s needs.

- **Calculated Measures**: This is a measure derived from the dataset to quantify specific insights related to vaccination or COVID-19 spread.

#### Model Optimization
- Ensured the fact table is structured efficiently for faster processing and analysis, reducing unnecessary complexity in the data model.

#### Report Enhancement
- Enhanced report visual appeal and readability by applying conditional formatting to highlight key trends (e.g., high case counts or vaccination rates).
- Added slicers and filters to allow for dynamic exploration of the data by different regions, dates, or metrics.
- Created bookmarks to easily navigate through different views of the report and save key filter settings for quick reference.

#### Advanced Analytics
- **Advanced Analytics Features Used**:
  - **Scatter with Animation**: Animated scatter plots to showcase trends over time (e.g., COVID-19 spread).
  - **Clustering**: Grouped countries or regions with similar characteristics for deeper insights.
  - **Q&A Functionality**: Enabled users to ask natural language questions about the data and get automated answers.
  - **Key Influencers**: Identified the key factors influencing vaccination rates or COVID-19 case counts.
  - **Decomposition Tree**: Used to break down data and understand the root causes of patterns in the dataset.
  - **Forecasting**: Implemented forecasting to predict future trends in COVID-19 cases or vaccination rates (max of 3 points for simplicity).
  - **Symmetry Shading**: Applied symmetry shading to highlight significant trends or anomalies in the data.

#### Dataset Management
- **Parameters Management**: Managed parameters for flexible data analysis and reporting, allowing users to adjust variables and customize views dynamically.

## Dashboards
- <a href="https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/global-covid-19_overview.png">Global Covid-19 Overview</a>
- <a href="[https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/global-covid-19_overview.png](https://github.com/ludreinsalvador/global-covid-19_data_analysis_dashboards/blob/main/global-vaccination_analysis.png)"></a>

