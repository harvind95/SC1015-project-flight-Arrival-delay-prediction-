# SC1015-project- flight Arrival delay prediction

*/to install type "pip install (install module name)"/*

Necessary libraries
 import pandas as pd
 import numpy as np
 import seaborn as sb
 from sklearn.model_selection import train_test_split 
 from sklearn.linear_model import LinearRegression
 from sklearn.linear_model import LogisticRegression
 from sklearn.ensemble import RandomForestClassifier
 from sklearn import metrics
 from sklearn.metrics import r2_score,mean_absolute_error,mean_squared_error
 import matplotlib.pyplot as plt


Problem statement
 To predict if the flight will be delayed

data cleaning
 we first clean the data to remove unneccesary column and remove unwanted data

data preprocessing
 we categorised time and months to 4 time frame and 4 seasons(explanation available in the notebook)
 
 we then did basic exploratory analysis on the dataset. however, due to the presence
 of negative values it is not entirely insightful although continuous data is necessary
 for linear regression modelling.

Modelling
 
 we first utilise Linear regression modelling to predict how long the delay will be
 if there happens to be a delay.

 However, the goal of this analysis is to predict whether there is a delay or not and not how 
 long a delay will be.

 Hence, the relevant numeric values(explained in notebook) are converted to categorical 
 dataset to suit our need.

 Exploratory data analysis is done again to understand the dataset further. These results 
 were better and significant amount of insights were gained.

 We then utilised logistic regression to predict arrival delay as this model better suits 
 categorical values.

 To further improve the accuracy we utilised decision tree modelling and also random forest 
 classifier modelling on the new data.

Conclusion

 In conclusion, to directly answer the question whether if the flight will be delayed? We 
 should deploy the random forest classifier and or logistic regression, which will return a 
 categorical answer. However, after much thought, linear regression model can also work if we 
 add a few more lines of code. Linear regression returns the duration of delay, a continuous value, 
 and we find that we can indirectly determine whether a flight will be delayed or not from this 
 outcome.

 Any of the above method will work, Random Forest Classifier and logistic regression will return results directly but linear 
 regression can show duration of delay, all with similar accuracy.
 
Contribution:
 Hard to specify as alot of discussion and work has been done across the requirement aspect.

Reference

Abdulhamit Subasi, 2020. Practical Machine Learning for Data Analysis Using Python

Edgar, T. W., & Manz, D. O. (2017). Exploratory Study. Research Methods for Cyber Security, 
95–130. https://doi.org/10.1016/b978-0-12-805349-2.00004-2‌

Dr. Sengupta, Sourav, 2022. Data Science and Artificial Intelligence. [Lab Materials] 
Nanyang Technological University, Singapore. 

Neil Liberman, 2017. Decision Trees and Random Forests. 
https://towardsdatascience.com/decision-trees-and-random-forests-df0c3123f991

sklearn.linear_model.LogisticRegression. (2014). Scikit-Learn. https://scikit-learn.org/stable/modules/
generated/sklearn.linear_model.LogisticRegression.html

sklearn.ensemble.RandomForestClassifier. (2022). Scikit-Learn. https://scikit-learn.org/stable/modules/
generated/sklearn.ensemble.RandomForestClassifier.html
