# House Price Prediction: Project Overview

* Created a tool that estimates house price (MAE ~ $16k) to help buyers negotiate the price when they have to buy one.
* Obtained the data from kaggle and used python as the programming langauge.
* Analysed which features corrleated most with price prediction.
* Gradient Boosting Regressor, Random Forest Regressor and Linear Regression models used to predict house prices.

## Software used
**Python Version:** 3.8.3 

**Packages used:** pandas,numpy,matplotlib,seaborn,sklearn

**IDE:** Jupyter Notebook

## Data cleaning
After obtaining the data from kaggle, I needed to clean it up so that it was usable for model. I made the following changes.
* Lot Frontage: There were missing values hence mean was calculated and replaced in those places.
* Electrical: Missing values were replaced by the most common observation(SBrkr).
* Remaining columns: Instead of **absent** the values put were **NaN** which resulted in inconsistency of the data.

## Model Building
First I split the numerical and categorical columns. The category dataframe was converted using dummy variables and again a model-ready dataframe was created by joining the two dataframes

I tried several different models however only 3 are listed for readability. Evaluation was doing using MAE as it is relatively easy to interpret
* Linear Regression
* Random Forest Regressor
* Gradient Boostin Regressor

## Model Performance
The Linear Regression model outperformed the others by a **HUGE** margin.
* Linear Regression: MAE = 16717
* Random Forest Regressor: MAE = 71371
* Gradient Boosting Regressor: MAE = 73071
