# SC1015 Mini Project: Life Expectancy
Lab Y127 
## About

In this data science project, we have used the World Health Organization (WHO) dataset on global health indicators to investigate the impact of various factors on life expectancy. The dataset contains a comprehensive collection of health-related indicators from year 2000-2015 for 193 countries, including socio-economic status, demographics, health behaviors, and conditions.

## Problem definition

Our precise problem statement is as follows:

We aim to analyze the WHO dataset to answer two research questions:

Do the initially chosen predicting factors have a significant effect on life expectancy, or do some of these factors have negligible influence?
Which variables are the most important predictors of life expectancy, and how can we identify and prioritize these key determinants?

## Motivation

The motivation behind this project is to gain a deeper understanding of the factors that influence life expectancy and use this knowledge to inform targeted and effective policy interventions. The project will also develop a predictive model that estimates an individual's life expectancy based on a chosen set of relevant factors. By identifying the most impactful variables, we can help governments, healthcare organizations, and communities make data-driven decisions to improve population health outcomes and reduce disparities in life expectancy across different regions.

## Dataset used


## Video presentation

## Project flow
[1. Data cleaning](https://github.com/TimSeaM/SC1015-Mini-Project-/blob/main/Data%20Cleaning.ipynb "1. Data cleaning")
   - Variable Name and Description
   - Abnormal & Missing values
   - Outliers
   - Preliminary look at dataset

[2. Exploratory Data Analysis (EDA) & Feature Engineering & Selection]
   - Histogram etc
   - Data altered etc

[3. Model Training 1 (Linear Regression)]
   - Test
     - Test
     - Results

[4. Model Training 2 (Polynomial Regression)](https://github.com/TimSeaM/SC1015-Mini-Project-/blob/main/Polynomial_Regression_Tim.ipynb "1. Data cleaning")
   - Definition
   - Pros and Cons
   - Degree comparison of Polynomial regression 
   - Train and test with "Income Composition of Resources"
     - Degree of 4 give the best results without overfitting
     - Accuracy: 69.5%

[5. Model Training 3 (Logistic Regression)]
   - ABC
   - Train and test with "Development" 
     - 
     - Accuracy: 92%

## Conclusion
- Income Composition of Resources and Schooling are the most important indicators of Life Expectancy. The closer both are to their respective max values, the better the Life Expectancy.
- Out of all the 3 models we implemented, Logistic Regression performed the best while Linear regression performed the worst.
- There is a clear indication that disease statistic, while an indicator of life expectancy, do not matter as much as the allocation of the countries' resources.

## Key learning points
- Data Cleaning
  - Interpolation
  - Winsorization (Limiting of outliers)
- EDA & Feature Engineering & Selection
  - 
- Linear Regression 
- Polynomial Regression
- Logistic Regression
## Contributors
(In alphabetical order)

Jeeho
- Data Cleaning, Linear Regression and Video Presenter 

Jenny
- Exploratory Data Analysis, Logistic Regression, Slides and script

Timothy Lim
- Polynomial regression, Feature Engineering & Selection, Collation & organisation on to Github, Slides and script
## References
