# Bike Sharing Demand Analysis

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Result and Findings](#result-and-findings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

### Project Overview

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. One main operational challenge is the redistribution logistics of bikes to maintain availability across the city. Solving this issue would allow rental bikes to be available to the public at the right time, lessening their waiting time. The following questions will be answered, which will provide impactful insights and recommendations for this problem.

### Objective

The objective of this analysis is to understand the trends in the data and identify key factors affecting the hourly demand for rental bikes.

### Exploratory Data Analysis

1. How does bike rental demand vary throughout the day?
2. How does bike rental demand vary with Season, Holiday, Functioning Day, etc?
3. Does bike rental demand have any correlation with any other numerical features?

### Data Sources

- **Data source:** <a href="https://archive.ics.uci.edu/dataset/560/seoul+bike+sharing+demand" target="_blank">UC Irving Machine Learning Repository</a>
- **Time period:** 2017-2018
- **Data size:** SeoulBikeData (8760, 14)
- **Key columns:** Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall, the number of bikes rented per hour and date information 
- **Calculated columns:** day of week, month, year, week
- [**Download Data set**](https://github.com/AaronW184/Seoul-Bike-Sharing-Demand/blob/main/SeoulBikeData.csv)

### Tools and Technologies used

The programming language used in this project is Python . The following libraries were used for data analysis and data visualization and to build a classifier to predict the price range of mobile phones.

Pandas : For loading the dataset and performing data wrangling

Matplotlib: For data visualization.

Seaborn: For data visualization.

NumPy: For some math operations in predictions.

### Steps Involved

1. Checked for outliers, incorrect values, missing values, duplicates and performed data type correction.

2. Created new columns such as Day, Month, Year, Days_of_week and week from Date column.
   
3. Exploratory Data Analysis : Performed Univariate, Bivariate, and Multivariate analysis with various graphs and plots to better understand the distribution of features and their relationships.

### Result and Findings

- Highest average bike rental demand at occurs at 6pm.

- Demand drops during Winter as temperatures falls to -2.54°C on average during Winter. 

- Demand picks up rapidly during office starting and ending hours during working days whereas it is popular in the afternoons and evenings during weekends.

- More people are adopting bike rental service as demand increase in 2018 compared to 2017.

### Recommendations

- Ensure more bikes are available around 6 pm, especially during weekdays, to meet the high demand.

- Provide heated docking stations or insulated bikes during winter to encourage usage despite lower temperatures.

- Place more bikes near office areas for morning and evening rush hours on working days, and in leisure spots for afternoons and evenings on weekends.

- Run promotional campaigns, providing incentives such as discounts or rewards to maintain usage levels during winter.

- Consider introducing more bikes to the city to accommodate the growing number of users.

### Limitations

- The number of holidays in a year is small hence constitute only 5% of the holiday feature. More data could be collected to improve the accuracy of the analysis that utilise this feature.
  
- The dataset spans only 2 years, which may not be sufficient to capture long-term trends or changes in bike-sharing demand.

### Further Steps

Implementing Predictive Machine Learning model, steps involved includes fixing certain features such as normalising skewed data, evaluating model using Train/Test data and cross validation, Improving model performance, etc. Accurately forecasting bike rental demand helps in managing the supply of bikes across different stations, ensuring availability when needed. Additionally, as bike-sharing systems expand, ML models can scale to accommodate larger datasets and provide more refined insights.
