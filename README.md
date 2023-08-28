# Final-Project-Statistical-Modelling-with-Python

## Project/Goals

In this project, the goal was to explore the relationship between bike availability at various stations in Toronto and the availability of parks using data from Foursquare and Yelp APIs. The project aimed to uncover potential insights regarding the impact of park availability on bike usage and explore statistical modeling techniques to analyze this relationship.

## Process

### Step 1: Data Collection and Exploration
1. Data Collection: Gathered data from CityBikes (https://citybik.es/), Foursquare and Yelp APIs to acquire information about bike stations, park counts, and average ratings.

2. Exploratory Data Analysis (EDA): Conducted exploratory analysis to understand initial patterns and relationships between bike availability, park counts, and ratings. Utilized visualizations such as scatter plots and bar plots to gain insights.

3. Initial Pattern Recognition: Identified a possible negative correlation between bike availability and total park counts using scatter plots and trend lines. Further statistical analysis was needed to validate this relationship.

4. Data Transformation: Managed outliers through Z-scores and applied a Yeo-Johnson transformation to address non-normality in the 'bikes' variable.

### Step 2: Modeling and Interpretation
1. Linear Regression Modeling: Built a linear regression model using 'fs_parks' and 'yelp_parks' as predictor variables and the transformed 'bikes' variable as the target. Analyzed the model's summary to understand predictor significance and explanatory power.

2. Hypothesis Testing: Conducted hypothesis testing to determine whether the number of available bikes is significantly affected by the number of Foursquare and Yelp parks. Evaluated p-values to assess predictor impact.

## Results

1. Initial Pattern/Relationship:
Based on the scatter plot and trend line, there's a potential negative correlation between bike availability and total park counts (Foursquare + Yelp) for bike stations. The scatter plot showed that higher bike availability tends to coincide with lower total park counts. The negative slope of the trend line supported this trend.

2. Linear Regression Model Analysis:
The linear regression model indicated that the predictor variables (fs_parks and yelp_parks) had limited explanatory power for bike availability. The R-squared value of 0.033 indicated that only around 3.3% of the variance in bike availability could be explained by the predictors. Both predictor coefficients had p-values above 0.05, suggesting no statistically significant impact.

3. Hypothesis Testing:
Hypothesis testing results suggested insufficient evidence to reject the null hypothesis that the number of available bikes is not significantly influenced by Foursquare and Yelp park counts. Both predictor variables exhibited p-values greater than 0.05, indicating limited impact on bike availability.

## Challenges 

The project faced challenges in handling outliers, addressing non-normality, and interpreting the significance of predictor variables. Additionally, the limited explanatory power of the linear regression model posed challenges in drawing definitive conclusions.

## Future Goals

Given more time, further exploration could involve incorporating additional variables, considering other regression techniques, and conducting more in-depth analysis to understand factors influencing bike availability and park counts more comprehensively.





