![](https://github.com/yeegorski/titanic_logistic/blob/master/titanic.png)
# Titanic: Machine Learning from Disaster
Here I present my solution to the famous Titanic machine learning competition.

* Performed the exploratory data analysis
* Performed data cleaning
* Engineered features from the existing variables
* Tested the data on Logistic, Support Vector, K-Nearest Neighbors, and Random Forest Regressors to reach the best accuracy score

## Code and Resources Used
**Python Version:** 3.7  
**Packages:** pandas, numpy, sklearn, matplotlib, seaborn  
**Data set:** https://www.kaggle.com/c/titanic

## EDA
I checked how complete the training data set was, and taking into account the missing data I pooled up some valuable information. Below are a few highlights:

![alt text](https://github.com/yeegorski/titanic_logistic/blob/master/age_sex_dist.png "Age Distribution by Sex and Survival")
![alt text](https://github.com/yeegorski/titanic_logistic/blob/master/pclass_countplot.png "Survivals by Passenger Class")
![alt text](https://github.com/yeegorski/titanic_logistic/blob/master/embark_countplot.png "Survivals by Port")

## Data Cleaning
* Created the *Title* variable by taking the passengers' titles from the *Name* variable
* Grouped the rare titles into one category (e.g. Lady, Sir, Major -> Rare), and renamed the French titles into the English ones (e.g. Mlle -> Miss, Mme -> Mrs)
* Imputed the missing *Age* values by imputing the average age of each passenger class and title group

## Model Building and Performance
* Transformed the categorical variables *Sex*, *Embarked*, *Title* into dummy variables
* Split the data into train and test sets with a test size of 30%

I tried four different models (along with the respective accuracy scores):
* **Logistic Regression**: 85.77%
* **Support Vector Machines**: 71.16%
* **K-Nearest Neighbors**: 71.54%
* **Random Forest**: 84.64%







