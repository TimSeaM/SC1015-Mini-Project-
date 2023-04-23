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

The motivation behind this project is to gain a deeper understanding of the factors that influence life expectancy and use this knowledge to inform targeted and effective policy interventions. The project will also use predictive models that estimates an individual's life expectancy based on a chosen set of relevant factors. By identifying the most impactful variables, we can help governments, healthcare organizations, and communities make data-driven decisions to improve population health outcomes and reduce disparities in life expectancy across different regions.

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
   - Tuning with Degree comparison of Polynomial regression 
   - Train and test with "Income Composition of Resources"
     - Degree of 4 give the best results without overfitting
     - Accuracy: 69.5%

[5. Model Training 3 (Logistic Regression)](https://github.com/TimSeaM/SC1015-Mini-Project-/blob/main/Logistic%20Regression%20Model.ipynb)
   - Definition
   - Model Evaluation
   - Tuning using GridSearchCV
   - Train and Test with "Development"
     - Custom Logistic Regression Model Summary
     - Accuracy: 94%

## Conclusion
- The initially chosen predicting factors all have a very big positive effect on life span. The closer to their upper limit they are, the higher the avg lifespan.
- There is a clear indication that disease statistic, while an indicator of life expectancy, do not matter as much as the allocation of the countries' resources.

- Income Composition of Resources is the most important indicator of Life Expectancy. The closer it is to the max values, the better the Life Expectancy.
- Out of all the 3 models we implemented, Logistic Regression performed the best at over 90% while Linear regression performed the worst at under 30%.
- This concludes that how a country uses its income, is the most important datapoint to extrapolate Life expectancy from. As "Income Composition of Resources" measures how good a country is at utilizing its resources, from 0 to 1, the closer it is to 1, the more efficient and effective that ultilisation is,thus the higher the country's life expectancy will be.

- The outcome of our project was the development of statistical models to analyze the relationship between life expectancy and various factors, such as a country's development status and income composition of resources. Although our models provided valuable insights, they did not fully solve the original problem, as there is still room for improvement in the accuracy of our predictions. However, our findings have laid a strong foundation for future research in this area.

Some interesting insights emerged from our analysis. In the polynomial regression model, we discovered that a polynomial function of degree 4 provided the most accurate and well-fitted model when relating the "Income_composition_of_resources" variable with life expectancy. This demonstrates the importance of selecting an appropriate degree for polynomial regression in order to avoid overfitting and underfitting issues.

Our logistic regression analysis revealed that higher life expectancy is associated with a higher likelihood of a country being classified as 'Developed,' while lower life expectancy is more likely to be associated with 'Developing' countries. This information can help inform policy interventions and resource allocation decisions in order to improve population health outcomes.

Based on our data-driven insights, we recommend that policymakers and healthcare organizations consider factors such as income composition of resources and development status when addressing life expectancy disparities. Further exploration of other models and variables may lead to even more accurate predictions and a deeper understanding of the factors that influence life expectancy. Ultimately, these insights can guide data-driven decisions to improve population health outcomes and reduce global disparities in life expectancy.

## Key learning points
- Data Cleaning
  - Interpolation
  - Tukey's method (Limiting of outliers)
  - Winsorization 
- EDA & Feature Engineering & Selection
  - Data selection based on Violin graph
- Polynomial Regression
  - Degree testing
  - Characteristics of under and over fitting
- Logistic Regression
  - Logistic Regression Model training
  - Model Tuning using GridSearchCV
## Contributors
(In alphabetical order)

Jeeho Lee
- Data Cleaning, Linear Regression, Video Presenter, Slides and Script

Timothy Lim
- Polynomial regression, Feature Engineering & Selection, Github coordination, Slides and Script

Xintong Zhang
- Exploratory Data Analysis, Logistic Regression, Slides and script

