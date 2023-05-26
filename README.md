# From-scraping-to-data-analysis-Glassdoor-website

A model is developed to estimate the salary in data science field.
Scraped 870 job positions from glassdoor using python and beautifulsoup.
Data cleaning, features engineering, model building, evaluating and tunning are done on the data.
Linear, Lasso, Polynomial, and Random Forest Regressors are considered and also GridsearchCV is used to reach the best model.



Code and Resources Used  :
 

Python Version: 3.7

Packages: pandas, numpy, sklearn, matplotlib, seaborn, beautifulsoup

 
 
Web Scraping  :
 

I scraped glassdoor.com using beautifulsoup and 870 job data were obtained. With each job, I got the following:

Job title

Salary

Rating of the company

Company name

City



Data Cleaning  :

 
After scraping the data, I needed to clean it up so that it was usable for our model. I made the following changes and created the following variables:

Parsed numeric data out of salary

Made a column for hourly wages

Removed rows without salary

Replaced missing values in rating variable with the mean of rating

Made a new column for company state

Column for simplified job title

Column for Seniority



EDA  :
 

I analyzed the variables using histograms, bar charts, box charts, scatter plots, and pivot tables.



Model Building  :


First, I transformed the categorical variables into dummy variables. I then split the data into train and tests sets with a test size of 20%.

I tried four different models and evaluated them using R2 score. I chose R2 because it is relatively easy to interpret.

I tried these four different models:

Multiple Linear Regression ,  Lasso Regression ,  Polynomial ,  Random Forest 

I also used K-Fold cross validation to check and compare the performance of different Machine Learning models.

Grid Search is also used in order to tune the parameters for Random Forest model.



Model performance  :


The Random Forest model outperformed the other models.







