# Phase-3-Telcom-Churn-Data-Analysis
## Overview
The telecommunication sector is a dynamic industry characterized by network infrastructure,technological innovation and global connectivity.However,customers may switch from one telecommunication service to another or they may discontinue the service altogether,a phenomenon called 'Telecom churn'.Telecom churn analysis is a crucial aspect of business intelligence for telecommunication companies as it helps them understand why customers are leaving and what actions can be taken to reduce churn rates.SyraiTel,a telecommunications company,has compiled data on their customers and whether or not they churned.In this project,we are looking to provide predictive and actionable insights regarding likely churn candidates at SyriaTel. We hope to create a complex model that can predict likely churn candidates as well as the features that impact churn the most.
## Business Understanding
The primary goal of this project is to to unlock actionable insights that will empower SyriaTel to implement targeted strategies to mitigate customer churn, ultimately fostering long-term business sustainability.To achieve this objective we need to develop a model that can identify the key factors influencing telecom churn. To effectively train this model, the client requires precise and representative data related to the customers of this telecommunications company.
Once trained the model will be capable of providing accurate predictions on whether customers will churn or not.
## Research Questions
1.Which features of the SyriaTel dataset are the most significant predictors of customer churn?  
2.How do various models differ in their ability to predict customer churn?  
3.How can SyriaTel mitigate customer churn?
## Data Understanding
The dataset used in this project was sourced from Kaggle (https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset).
The columns that have been used in the dataset are:  
state:The state the customer lives in.  
account length:The number of days a customer has had an account.  
phone number: the phone number of the customer.  
international plan: true if the customer has the international plan, otherwise false.  
voice mail plan: true if the customer has the voice mail plan, otherwise false.  
number vmail messages: the number of voicemails the customer has sent.  
total day minutes: total number of minutes the customer has been in calls during the day.  
total day calls: total number of calls the user has done during the day.  
total day charge: total amount of money the customer was charged by the Telecom company for calls during the day.  
total eve minutes: total number of minutes the customer has been in calls during the evening.  
total eve calls: total number of calls the customer has done during the evening.  
total eve charge: total amount of money the customer was charged by the Telecom company for calls during the evening.  
total night minutes: total number of minutes the customer has been in calls during the night.  
total night calls: total number of calls the customer has done during the night.  
total night charge: total amount of money the customer was charged by the Telecom company for calls during the night.  
total intl minutes: total number of minutes the user has been in international calls.  
total intl calls: total number of international calls the customer has done.  
total intl charge: total amount of money the customer was charged by the Telecom company for international calls 
customer service calls: number of calls the customer has made to customer service.  
churn: true if the customer terminated their contract, otherwise false.
## Data preparation
We can drop columns which do not provide information which is necessary.In this case we can drop the following columns:

- Phone Number.    
- Number of voice mail messages.  
- Area code.
The dataset has no null values or duplicates.
## Exploratory Data Analysis
The following visulaizations were created to explore the data:  
- A pie chart showing percentage of customers who churned against customers who did not churn.
- Bar plot showing frequency of customers who churned against customers who did not churn.
- Bar plot showing frequency of customers who have an international plan against customers who do not have an international plan.
- Bar plot showing frequency of customers who have a voice mail plan against customers who do not have a voice mail plan.
- Bar plot showing the relationship between churn and international plan.
- Bar plot showing the relationship between churn and voice mail plan.
- Bar plot showing the top 5 states for churned customers.
- Bar plot showing the bottom 5 states for non-churned customers.
- Bar plot showing the top 5 states for churned customers.
- Bar plot showing the bottom 5 states for non-churned customers.
- A correlation heatmap showing the relationship between all numerical variables.
- Histograms  showing the frequency distribution of day,evening and night calls.
- Bar plot counting the frequency of customer service calls.
## Modelling
Three classification models were built:  
- Logistic Regression model.
- Decision Tree Classifier.
- Random  forest Classifier.
## Conclusion
We can now conclude that a random forest model provides better insights into this dataset than a decision tree or a logistic regression model,even without tuned hyperparameters.The feature importance bar graph shows that total day minutes,total day charge and customer service calls are the features which influence whether customers churn or not.
## Recommendations
- Imporve their products' reliability to reduce the number of customer service calls.Once customers call 4/5 times plus,they are likely to churn.
- Promote their products more aggressively in the states of New Jersey,Texas,Maryland,Michigan and New York.A huge number of their churned customers reside in these states.
- Reduce their charges for international calls.Not many of the customers have an international plan.
- Provide discounts on charges for day calls as it influences whether customers churn or not significantly.
