# Course #5: Statistics for Data Science with Python

<p align = "center">
<img src = "statistics-for-data-science-with-python.png">
</p>

## Project: Statisitcal Analysis of the Boston Housing Dataset
**Project Scenario**: You are working as a Data Scientist with a housing agency in Boston MA. You have been given access to a previous dataset on housing prices derived from the U.S. Census Service to present insights to higher management. Based on your experience in Statistics, what information can you provide them to help with making an informed decision? Upper management will like to get some insight into the following.

- Is there a significant difference in the median value of houses bounded by the Charles river or not?
- Is there a difference in median values of houses of each proportion of owner-occupied units built before 1940?
- Can we conclude that there is no relationship between Nitric oxide concentrations and the proportion of non-retail business acres per town?
- What is the impact of an additional weighted distance to the five Boston employment centres on the median value of owner-occupied homes?
<br><br>

The notebook for this project can be accessed here.


### About the dataset

The dataset can be find here: [Boston Housing Dataset](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-ST0151EN-SkillsNetwork/labs/boston_housing.csv)

The following describes the data variables:

-      CRIM - per capita crime rate by town

-      ZN - proportion of residential land zoned for lots over 25,000 sq.ft.

-      INDUS - proportion of non-retail business acres per town.

-      CHAS - Charles River dummy variable (1 if tract bounds river; 0 otherwise)

-      NOX - nitric oxides concentration (parts per 10 million)

-      RM - average number of rooms per dwelling

-      AGE - proportion of owner-occupied units built prior to 1940

-      DIS - weighted distances to five Boston employment centres

-      RAD - index of accessibility to radial highways

-      TAX - full-value property-tax rate per $10,000.

-      PTRATIO - pupil-teacher ratio by town

-      LSTAT - % lower status of the population

-      MEDV - Median value of owner-occupied homes in $1000's

### Exploratory Data Analysis (EDA)

<img src = "MEDV barplot.png">
<img src = "MEDV boxplot.png">
<img src = "MEDV based on age_group.png">
<img src = "NOX vs INDUS.png">
<img src = "PTRATIO histogram.png">

### Conclusion
- There is a significant different in the median value of houeses bounded/non-bounded Charles River 
- There is a significant difference in median values of houses of each proportion of owner-occupied units built before 1940 
- There exists a relationship between the variables NOX and INDUS
- The average change in the value of owner-occupied homes (in $1000's) increased the weighted distances to five Boston employment centres by 1.0916








