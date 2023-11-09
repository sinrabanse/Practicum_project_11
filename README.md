# Practicum_project_11
 My eleventh project from Practicum course

 What was used in the project: Python, Jupyter notebook. Libraries: pandas, matplotlib, seaborn, sklearn.

Project Description

I am data analyst in the gym chain Model Fitness. In order to fight churn, Model Fitness has digitized a number of its customer profiles. My task is to analyze them and come up with a customer retention strategy.

I should:
 - Learn to predict the probability of churn (for the upcoming month) for each customer
 - Draw up typical user portraits: select the most outstanding groups and describe their main features
 - Analyze the factors that impact churn most
 - Draw basic conclusions and develop recommendations on how to improve customer service

# Steps
1) Carry out exploratory data analysis (EDA):
   - Look at the dataset: does it contain any missing features?
   - Look at the mean feature values in two groups: for those who left (churn) and for those who stayed.
   - Plot bar histograms and feature distributions for those who left (churn) and those who stayed.
   - Build a correlation matrix and display it.
2) Build a model to predict user churn:
   - Divide the data into train and validation sets using the train_test_split() function.
   - Train the model on the train set with two methods:
        - logistic regression
        - random forest
   - Evaluate accuracy, precision, and recall for both models using the validation data. Use them to compare the models. Which model gave better results?
3) Create user clusters:
   - Standardize the data.
   - Use the linkage() function to build a matrix of distances based on the standardized feature matrix and plot a dendrogram.
   - Train the clustering model with the K-means algorithm and predict customer clusters.
   - Look at the mean feature values for clusters.
   - Plot distributions of features for the clusters.
   - Calculate the churn rate for each cluster
4) Conclusions and basic recommendations on working with customers

# Description of the data
The data is stored in the file gym_churn_us.csv

## Description of columns:
'Churn' - the fact of churn for the month in question<br/>
'gender'<br/>
'Near_Location' - whether the user lives or works in the neighborhood where the gym is located<br/>
'Partner' - whether the user is an employee of a partner company (the gym has partner companies whose employees get discounts)<br/>
'Promo_friends' - whether the user originally signed up through a "bring a friend" offer<br/>
'Phone' - whether the user provided their phone number<br/>
'Age'<br/>
'Lifetime' - the time (in months) since the customer first came to the gym<br/>
Data from the log of visits and purchases and data on current membership status<br/>
'Contract_period' - 1 month, 3 months, 6 months, or 1 year<br/>
'Month_to_end_contract' - the months remaining until the contract expires<br/>
'Group_visits' - whether the user takes part in group sessions<br/>
'Avg_class_frequency_total' - average frequency of visits per week over the customer's lifetime<br/>
'Avg_class_frequency_current_month' - average frequency of visits per week over the preceding month<br/>
'Avg_additional_charges_total' - the total amount of money spent on other gym services: cafe, athletic goods, cosmetics, massages, etc.
