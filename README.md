# World_Happiness_Analysis

## Overview
This project presents a detailed analysis of the World Happiness Reports from 2015 to 2019, aiming to understand the factors contributing to the happiness of citizens across different countries. The World Happiness Report, often subject to debate regarding its metrics, attempts to quantify global perceptions of happiness and identify key contributors to individual and societal well-being. This analysis scrutinizes these metrics to assess their validity and impact on overall happiness scores.

## Objectives
- To explore what makes citizens content with their country and identify major contributors to happiness.
- To examine the metrics of the World Happiness Reports critically and evaluate if criticisms of these measurements are valid.
- To use geographic mapping for a holistic view of global happiness trends and identify patterns between countries.

## Dataset
The dataset used in this project includes the World Happiness Reports from 2015 to 2019, sourced from Kaggle. Each year's report comprises various metrics, such as GDP per capita, family support, life expectancy, freedom, trust in government, and generosity, contributing to a country's overall happiness score.

**Dataset Link:** https://www.kaggle.com/datasets/unsdsn/world-happiness

**Columns:**

- **Country:** The country's name.
- **Region:** The geographic region to which the country belongs.
- **Happiness Rank:** The rank of the country based on the Happiness Score.
- **Happiness Score:** A metric measured by asking sampled people to rate their happiness on a scale of 0 to 10.
- **Standard Error:** The standard error of the happiness score.
- **Economy (GDP per Capita):** Contribution of GDP to the Happiness Score.
- **Family:** Contribution of family support to the Happiness Score.
- **Health (Life Expectancy):** Contribution of life expectancy to the Happiness Score.
- **Freedom:** Contribution of freedom to the Happiness Score.
- **Trust (Government Corruption):** Contribution of the perception of corruption to the Happiness Score.
- **Generosity:** The extent of generosity in the country.

## Libraries and Tools 
- **Data Manipulation:** pandas, numpy
- **Data Visualization:** seaborn, matplotlib, plotly
- **Geospatial Analysis:** mpl_toolkits.basemap
- **Statistical Analysis:** scipy.stats
- **Data Profiling:** pandas_profiling
- **Country Data Management:** pycountry

## Data Processing
- **Data Loading:** Separate datasets for each year (2015-2019) were loaded into Pandas dataframes.
- **Data Standardization:** Given the variations in dataset formats across years, a custom function parse_report was used to standardize and combine datasets. This function renames columns for consistency, calculates quartiles, and appends a 'Year' column.
- **Data Cleaning:** Renaming and correcting country names for accurate mapping and analysis. The project also addresses missing values and inconsistencies across different report formats.

## Exploratory Data Analysis (EDA)
- **Descriptive Statistics:** The describe method provided a statistical summary of the dataset, giving insights into the mean, standard deviation, and quartile distribution of each metric.
- **Data Visualization:** Various plots, including histograms and pair plots, were created to understand distributions and relationships between different variables. Histograms were enhanced with fitted normal distributions to assess the deviation from normality.
- **Correlation Analysis:** An annotated heatmap was used to analyze correlations between different variables, highlighting relationships crucial for understanding what influences happiness scores.

## Interactive Data Visualization and Geospatial Analysis
1. Interactive Plots: Utilizing plotly, interactive scatter plots were created to dynamically explore relationships between variables over the years.
2. Geospatial Mapping:
   - Basemap: Used for creating global and regional maps, highlighting how different happiness metrics vary across countries.
   - Plotly Maps: Enhanced visualizations with animated choropleth maps, providing an interactive way to observe changes over the years.


