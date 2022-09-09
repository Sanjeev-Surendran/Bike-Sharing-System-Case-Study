# Bike Sharing System Case Study
A case study to solve a business problem by building a multiple linear regression model for the prediction of demand for shared bikes.
* Comprehend the given data set and perform Exploratory Data Analysis (EDA) to analyse the data set.
* Build multiple linear regression model to identify the best fit variables that can predict the demand for shared bikes.

## Table of Contents
* [General Info](#general-information)
* [Project Contents](#project-contents)
* [Conclusion](#conclusion)
* [Software and Library Versions](#software-and-library-versions)
* [Acknowledgements](#acknowledgements)

### General Information
A US bike-sharing provider **BoomBikes** provides service in which bikes are made available for shared use to individuals on a short-term basis for a price or free. Company allows people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

The company has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic and is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, company aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all-around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
* Which variables are significant in predicting the demand for shared bikes.
* How well those variables describe the bike demands

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

#### Data Set Brief Information
The data set contains information about the number of bike rentals during various environment factors, holidays, working day, weekends and across month and year (from 2018 to 2019). The data set contains
* Numerical Variables
* Categorical variables represented as numbers

A data dictionary is provided along with the data set to understand various terms and variables used.

In the dataset provided, there are three columns named 'casual', 'registered', and 'cnt'.
* The variable 'casual' indicates the number casual users who have made a rental.
* The variable 'registered' indicates the total number of registered users who have made a booking on a given day.
* Finally, the 'cnt' variable indicates the total number of bike rentals, including both casual and registered.

#### Business Objective
Analyse and Perform Exploratory Data Analysis (EDA) on the given data set. Build a multiple linear regression model to identify the best fit variables that can predict the demand for shared bikes ('cnt' as target variable).

#### Business Solution
Present the model, which can predict the number of bike rentals. BoomBikes management will use this model to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.


### Project Contents
* **Bike Sharing System Case Study.ipynb** - Jupyter Notebook for Bike Sharing System Case Study (Language : Python)
* **Linear Regression Subjective Questions.pdf** - Questions and Answers to subjective questions related to linear regression
* **day.csv** - Data Set
* **day_dictionary.txt** - Data Dictionary
* **README.md** - Readme file
* **.ipynb_checkpoints** - A folder with last saved contents of Jupyter Notebook.


### Conclusion
Any business analytics problem can be solved using **CR**oss **I**ndustry **S**tandard **P**rocess for **D**ata **M**ining (CRISP-DM) model.
* Data set was analysed and prepared for EDA. Univariate and Bivariate analysis were done on data set to understand the relationship between variables.
* Multiple Linear Regression model was built for target variable 'cnt' using both coarse tuning (Recursive Feature Elimination (RFE) method) and fine tuning (p-value and Variance Inflation Factor (VIF) method)

#### Recommendation
##### Linear Regression Model Summary Statistics of Train and Test Data
* Train R^2 : **0.836**
* Train Adjusted R^2 : **0.832**
* Test R^2 : **0.795**
* Test Adjusted R^2 : **0.785**
* This seems to be a really decent model that differentiate the dataset and can predict the variable 'cnt'.

##### Top predictor variables
* **Temperature (temp)** : coefficient value of 0.55. As temperature variable increases bike rentals increases by 0.55 units, provided all other predictor variables are constant.
* **Year (yr)** : coefficient value of 0.23. Bike rentals can increase by 0.23 units / year, provided all other predictor variables are constant.
* **Weather Situation 3 (weathersit_3)** : coefficient value of -0.29. When weather is either Light Snow or Light Rain + Thunderstorm + Scattered clouds or Light Rain + Scattered clouds, bike rentals can decrease by 0.29 units, provided all other predictor variables are constant.


### Software and Library Versions
* ![Jupyter Notebook](https://img.shields.io/static/v1?label=Jupyter%20Notebook&message=4.9.2&color=blue&labelColor=grey)

* ![NumPy](https://img.shields.io/static/v1?label=numpy&message=1.21.5&color=blue&labelColor=grey)

* ![Pandas](https://img.shields.io/static/v1?label=pandas&message=1.4.2&color=blue&labelColor=grey)

* ![matplotlib](https://img.shields.io/static/v1?label=matplotlib&message=3.5.1&color=blue&labelColor=grey)

* ![seaborn](https://img.shields.io/static/v1?label=seaborn&message=0.11.2&color=blue&labelColor=grey)

* ![statsmodels](https://img.shields.io/static/v1?label=statsmodels&message=0.13.2&color=blue&labelColor=grey)

* ![sklearn](https://img.shields.io/static/v1?label=sklearn&message=1.0.2&color=blue&labelColor=grey)


### Acknowledgements
This case study is an assignment, done as part of [Upgrad](https://www.upgrad.com/ ) - **Master of Science in Machine Learning & Artificial Intelligence** programme.


### Contact
Created by [Sanjeev Surendran](https://github.com/Sanjeev-Surendran)


<!-- ## License -->
<!-- This project is not a open source and sharing the project files is prohibited. -->
