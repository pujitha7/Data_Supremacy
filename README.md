# Data_Supremacy

# PROBLEM STATEMENT:

A training institute which conducts training for analytics/ data science wants to expand their business to manpower recruitment (data science only) as well. 
 
Company gets large number of signups for their trainings. Now, company wants to connect these enrollees with their clients who are looking to hire employees working in the same domain. Before that, it is important to know which of these candidates are really looking for a new employment. They have student information related to demographics, education, experience and features related to training as well.
 
To understand the factors that lead a person to look for a job change, the agency wants you to design a model that uses the current credentials/demographics/experience to predict the probability of an enrollee to look for a new job.

# INPUT VARIABLES:

Demographics, Education, Experience, etc

# TARGET VARIABLE:

0 - Not looking for job change
1 - Looking for job change

# METRIC:

AUC-ROC Score

# APPROACH:

A lot of preprocessing has been done to fill NAN values.

It is a Class-imbalanced classification problem.

Random Forest model is built with best parameters obtained from Grid Search.

LSTM model with online learning is built with custom loss function giving more penalty for rare class.

Random Forest was able to predict majority class well and LSTM model was able to predict minority class well so both of them are stacked to get a better model.




