# COVID-19 Data Analysis Project
This project analyzes the global spread and impact of the COVID-19 pandemic using publicly available datasets. It combines data on COVID-19 cases from Johns Hopkins University with socio-economic indicators from the World Happiness Report to explore potential correlations between a country's socio-economic factors (such as GDP, social support, and life expectancy) and its infection rates.

## Objective
The main goal of this project is to:

- Analyze the number of confirmed COVID-19 cases, recoveries, and deaths across countries and regions.
- Visualize the spread of the virus in specific countries (e.g., China).
- Investigate potential correlations between COVID-19 infection rates and various socio-economic factors like GDP, social support, and healthy life expectancy.

## Datasets Used
1. Johns Hopkins University COVID-19 Dataset:
- Source: Johns Hopkins University COVID-19 GitHub Repository
- Contains global data on confirmed COVID-19 cases, recoveries, and deaths.

2. World Happiness Report Dataset:
- Source: Kaggle
- Contains socio-economic indicators such as GDP per capita, social support, healthy life expectancy, freedom to make life choices, and overall happiness scores.

## Project Workflow

1. Loading the Datasets:
- Imported the COVID-19 data and World Happiness Report data using pandas.

2. Data Cleaning:
- Removed irrelevant columns such as latitude and longitude from the COVID-19 dataset as they were not necessary for this analysis.
- Aggregated data by Country/Region to summarize the total cases for each country.

3. Visualizing the Spread:
- Plotted the initial spread of the virus in China by examining the first 5 days of the pandemic and calculating the daily increase in cases using the .diff() function.
- Visualized the first derivative of the curve to observe the rate of new cases.

4. Calculating Maximum Infection Rates:
- Calculated the maximum daily new cases for each country to analyze the peak infection rates.

5. Happiness Correlation Analysis:
- Merged the COVID-19 dataset with the World Happiness Report dataset to investigate the relationship between happiness indicators and maximum infection rates.
- Selected relevant columns such as GDP per capita, social support, healthy life expectancy, and freedom to make life choices.

6. Correlation Matrix:
- Calculated the correlation between maximum infection rates and various happiness metrics using data.corr().

7. Data Visualization:
- Created scatter plots and regression plots to visualize the relationships between:
- GDP per capita vs. maximum infection rate
- Social support vs. maximum infection rate
- Healthy life expectancy vs. maximum infection rate
- Freedom to make life choices vs. maximum infection rate

## Key Insights
#### Significant Correlations: 
The analysis revealed significant correlations between certain socio-economic indicators (like GDP and social support) and infection rates. Countries with higher GDP and better social support tended to manage the pandemic better.
### Visualizations: 
The scatter and regression plots helped in understanding how factors like GDP and life expectancy are related to the spread of COVID-19.
New Cases in China: By calculating the first derivative of the infection curve, we visualized how new cases were increasing at the start of the pandemic, providing insight into the initial growth pattern.

## Tools and Technologies
Python: The project was implemented using Python.
Libraries:
- pandas for data manipulation and analysis.
- matplotlib and seaborn for data visualization.
Data Cleaning & Aggregation: Grouped data by country/region and cleaned datasets by removing unnecessary columns.
Correlation Matrix & Plots: Used the correlation matrix to uncover relationships and created scatter and regression plots for visualization.


## Conclusion
This project provided valuable insights into how socio-economic factors influence the spread of the COVID-19 pandemic. By merging health data with happiness metrics, we could explore correlations that may inform future public health policies. The analysis also highlights the importance of factors like GDP and social support in mitigating the impact of global health crises.
