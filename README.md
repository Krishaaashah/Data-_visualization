# Tracking Sustainable Urban Mobility: A Data-Driven Approach to Reduce Carbon Emissions

## Overview
This project presents an end-to-end analytical and predictive system for understanding and forecasting global CO₂ emissions. Using Power BI and R, the project converts raw datasets from multiple countries into interactive dashboards, advanced DAX calculations, and machine learning-driven forecasts to support environmental decision-making.

---

## Key Features
- Multi-country CO₂ emission analysis  
- Global and region-wise dashboards  
- Country-level trend and hotspot identification  
- Comparative emissions across countries and sectors  
- Predictive modeling with R (Linear Regression and Random Forest)  
- Time intelligence functions with custom Date Table  
- DAX-driven insights including CAGR, YOY, rankings, and rolling averages  
- Clean and optimized Power BI data model

---

## Problem Statement
Global CO₂ emissions continue to rise unevenly across nations, but there is no single interactive platform capable of analyzing, comparing, and forecasting emission trends with accuracy.  
This project addresses that gap by building a unified analytical dashboard supported by machine learning forecasts.

---

## Objectives
- Visualize historical CO₂ emission trends globally and per country  
- Compare emissions across countries, regions, and sectors  
- Forecast future emissions using R-based ML models  
- Provide advanced DAX-driven insights  
- Transform raw datasets into a decision-support platform for climate action  

---

## Dataset Summary
The dataset contains CO₂ emission statistics for ten countries:

- India  
- United States  
- United Kingdom  
- Germany  
- Italy  
- Japan  
- Russia  
- Brazil  
- South Africa  
- Nigeria  

Sources: World Bank, Our World in Data.

Data points include:  
- Total CO₂ emissions  
- Emissions per capita  
- Energy consumption indicators  
- Yearly time-series values  

---

## Data Preprocessing
Key preprocessing steps:

- Removal of duplicates and imputation of missing values  
- Standardization of numeric and categorical fields  
- Formatting dates into YYYY-MM-DD  
- Creating a Date Table for time intelligence  
- Merging individual country datasets into a master dataset  
- Handling outliers  
- Structuring fields for modeling and visualization  

---

## Data Model

### Fact Table
**Fact_Emissions**  
Contains:
- Total Emission  
- Emission Per Capita  
- Energy Consumption  
- Year  
- CountryID  
- DateKey  

### Dimension Tables
- **Dim_Country:** country, region, continent  
- **Dim_Date:** year, month, quarter, date hierarchy  
- **Dim_Sector:** sector classification (where applicable)

### Relationships
- CountryID and DateKey used as primary–foreign key relationships  
- One-to-many relationships support accurate filtering and drill-down analysis  

---

## DAX Measures Implemented
- Total CO₂ Emission  
- Emission Per Capita  
- Year-over-Year (YOY) Change  
- CAGR  
- Rolling 3-Month and 12-Month Averages  
- Emission Ranking by Country  
- Top Emitting Country  
- Custom Date Table (CALENDAR)  

These measures support trend analysis, forecasting integration, and time intelligence.

---

## Dashboards Developed

### 1. Global CO₂ Emission Dashboard
- World map visualization  
- Total emission KPIs  
- Moving averages  
- Z-score anomaly analysis  
- Global trendlines  

### 2. Country-Specific Dashboards
For each of the ten countries:  
- CO₂ emission trends  
- Regional distribution (donut charts)  
- Seasonal and long-term variations  
- Emission hotspots on map visuals  

### 3. Comparative Analysis Dashboard
- Country ranking (highest to lowest emitters)  
- Sector-wise emission breakdown (power, industry, residential, aviation, transport)  
- Cross-country visualization for emissions contribution  

### 4. Forecasting Dashboards (R Integration)
- Predicted vs actual graph  
- YOY forecast  
- Rolling 12-month moving average  
- Long-term trend projections  

---

## R Integration and Forecasting

### Models Used
1. **Linear Regression**
   - R²: 0.986 – 0.993  
   - Low RMSE values  
   - Highly reliable for linear trends  

2. **Random Forest Regression**
   - R²: 0.889 – 0.898  
   - Captures non-linear patterns  
   - Robust for real-world variations  

### Forecast Outputs
- Emission predictions for upcoming years  
- Rolling averages and YOY forecast bars  
- Model accuracy comparisons displayed directly in Power BI  

---

## Insights

### Global Trends
- The United States, China, and India are the largest contributors to global CO₂ emissions.  
- European countries (Germany, Italy, UK) show declining trends due to renewable energy policies.  
- Developing countries display increasing emissions driven by industrialization.

### Sector-Level Insights
- Power and Transport sectors contribute the highest share.  
- Residential and aviation sectors contribute comparatively lower emissions.  

### Forecasting Insights
- Emissions are projected to rise steadily.  
- Stabilization is expected after 2035 if current policies continue.

---

## Conclusion
The project demonstrates how combining analytics, visualization, and machine learning can produce powerful insights into global CO₂ emissions. Using Power BI and R, the solution provides descriptive, comparative, and predictive intelligence, supporting environmental scientists, policymakers, and organizations in planning sustainable development strategies.

---

## Technologies Used
- Power BI  
- Power Query  
- DAX  
- R Programming  
- Machine Learning (Linear Regression, Random Forest)  
- Star Schema Data Modeling  


---
