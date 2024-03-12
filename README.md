# Consumer Credit Analytical Model

## Overview

The objective of this project is to develop a robust analytical model capable of understanding the dynamics of consumer credit. We aim to investigate historical trends in consumer credit from June 2000 through December 2022 and utilize this data to predict future patterns up to December 2023. Through meticulous data preprocessing, exploratory analysis, and advanced predictive modeling techniques, we intend to offer valuable insights into the factors driving changes in consumer credit levels. By focusing on several key variables, such as interest rates, election cycles, and unemployment rates, we will determine their correlation and impact on consumer credit behavior. This analysis will not only allow us to predict the 'Total Consumer Credit' with a significant degree of accuracy but will also enable financial institutions to make informed decisions regarding credit risk management and policy development. By achieving our goal of a minimum of 0.80 R-squared value, we will ensure the reliability and effectiveness of our predictive model, providing a dependable tool for economic analysts and decision-makers.

## Data Source

- Bureau of Labor Statistics Data
- Consumer Credit - Data.gov
- Consumer Credit Trends

## Preprocessing the Data

- The data in CSV was formatted in Excel before analyzing the data in Python

## Setting up the Environment and Staging for the Prediction

- Used Google Colab
- Installed libraries required including PySpark and Java
- Used PySpark to fetch the dataset from Github via the URL link
- Converted to Pandas Dataframe
	
## Exploratory Data Analysis (EDA)

- Performed an EDA to make sense of the data trends through visualization
- Created a time series graph to show how consumer credit has evolved
	
## Correlation Matrix

- Utilized a correlation matrix to determine any relationsip between the Total Consumer Credit and the other features

## Analysis Results

- Used StandardScaler to normalize the features
- Used a Linear Regression model
- Trained the model using data prior to 2023, and tested it on data from 2023
- Created a comparison_df to compare the predicted and actual data from 2023
- Resulting r-squared value = 0.9855801997414367

## Impacts of Different Features

- Used coefficients from Linear Regression model and mapped them to different features to determine impacts:
{'Interest Rate': -0.000652273086771723,​
'Elections (yes/no)': -0.000244140625,​
'Inflation Rate': -3.0517578125e-05, ​
'Unemployment Rate': -0.000732421875, ​
'Motor Vehicle Loans Owned and Securitized': 227859742057.17444, ​
'Credit Cards and Other Revolving Plans': 220316388370.26282, ​
'Student loans': 5894479882.94339, ​
'Mortgages': 89403943591.27307, ​
'Other': 450673606701.9846}​
