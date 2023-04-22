# SC1015 Mini Project: Life Expectancy
Lab Y127 
## About

In this data science project, we have used the World Health Organization (WHO) dataset on global health indicators to investigate the impact of various factors on life expectancy. The dataset contains a comprehensive collection of health-related indicators from year 2000-2015 for 193 countries, including socio-economic status, demographics, health behaviors, and conditions.

## Problem definition

Our precise problem statement is as follows:

We aim to analyze the WHO dataset to answer two research questions:

Do the initially chosen predicting factors have a significant effect on life expectancy, or do some of these factors have negligible influence?
Which variables are the most important predictors of life expectancy ? and are they necessarily disease related ?

## Motivation

The motivation behind this project is to gain a deeper understanding of the factors that influence life expectancy and use this knowledge to inform targeted and effective policy interventions. The project will also develop a predictive model that estimates an individual's life expectancy based on a chosen set of relevant factors. By identifying the most impactful variables, we can help governments, healthcare organizations, and communities make data-driven decisions to improve population health outcomes and reduce disparities in life expectancy across different regions.

## Dataset used

The dataset used for this project is retrieved from [here](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who)

Datasets used and produced are uploaded here as "Life Expectancy Data.csv" and "CleanedLifeExpectancy.csv"

## Video presentation

## Project flow
[1. Data cleaning](https://github.com/TimSeaM/SC1015-Mini-Project-/blob/main/Data%20Cleaning.ipynb )
   - Variable Name and Description
   - Abnormal & Missing values
   - Outliers
   - Preliminary look at dataset

[2. Exploratory Data Analysis (EDA) & Feature Engineering & Selection](https://github.com/TimSeaM/SC1015-Mini-Project-/blob/main/Exploratory%20Data%20Analysis.ipynb)
   - Visualisation of Life Expectancy
   - Corrolation matrix & Heat map
   - Visualisation of selected variables

[3. Model Training 1 (Linear Regression)](https://github.com/TimSeaM/SC1015-Mini-Project-/blob/main/Linear_Regression_Jeeho.ipynb)
   - Pros and Cons
   - Linear regression
     - "GDP" with "Life expectancy"
     - Accuracy: 27.26%

[4. Model Training 2 (Polynomial Regression)](https://github.com/TimSeaM/SC1015-Mini-Project-/blob/main/Polynomial_Regression_Tim.ipynb )
   - Definition
   - Pros and Cons
   - Degree comparison of Polynomial regression 
   - Train and test with "Income Composition of Resources"
     - Degree of 4 give the best results without overfitting
     - Accuracy: 69.5%

[5. Model Training 3 (Logistic Regression)]
   - ABC
   - Train and Test with "Development"
     - Accuracy: 92%

## Analysis
IDK if this is needed?
## Conclusion
- The initially chosen predicting factors all have a very big positive effect on life span. The closer to their upper limit they are, the higher the avg lifespan.
- There is a clear indication that disease statistic, while an indicator of life expectancy, do not matter as much as the allocation of the countries' resources.

- Income Composition of Resources is the most important indicator of Life Expectancy. The closer it is to the max values, the better the Life Expectancy.
- Out of all the 3 models we implemented, Logistic Regression performed the best at over 90% while Linear regression performed the worst at under 30%.
- This concludes that how a country uses its income, is the most important datapoint to extrapolate Life expectancy from. As "Income Composition of Resources" measures how good a country is at utilizing its resources, from 0 to 1, the closer it is to 1, the more efficient and effective that ultilisation is,thus the higher the country's life expectancy will be.

## Key learning points
- Data Cleaning
  - Interpolation
  - Turkey's method (Limiting of outliers)
  - Winsorization 
- EDA & Feature Engineering & Selection
- Linear Regression 
- Polynomial Regression
- Logistic Regression
## Contributors
(In alphabetical order)

Jeeho Lee
- Data Cleaning, Linear Regression, Video Presenter, Script

Timothy Lim
- Polynomial regression, Feature Engineering & Selection, Github coordination, Script

Xintong Zhang
- Exploratory Data Analysis, Logistic Regression, Slides and script
## References
