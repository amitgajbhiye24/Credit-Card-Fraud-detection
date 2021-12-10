**Credit Card Fraud Detection**
***Problem statement***
In this project we need to predict fraudulent credit card transactions with the help of machine learning models.

we will analyse customer-level credit card transactional data which has been collected by bank and provide us to analyse.

The dataset is taken from the Kaggle Website and it has a total of 2,84,807 rows and 31 columns.

Out of total transactional cases 492 are fraudulent cases. Since the dataset is highly imbalanced,we needs to be handled and ballenced before model building.

**Business Problem Overview**
For many banks, retaining high profitable customers is the number one business goal. Banking fraud, however, poses a significant threat to this goal for different banks. In terms of substantial financial losses, trust and credibility, this is a concerning issue to both banks and customers alike.

It has been estimated by Nilson report by 2020 the banking frauds would account to $30 billion worldwide. With the rise in digital payment channels, the number of fraudulent transactions is also increasing with new and different ways.

In the banking industry, credit card fraud detection using machine learning is not just a trend but a necessity for them to put proactive monitoring and fraud prevention mechanisms in place. Machine learning is helping these institutions to reduce time-consuming manual reviews, costly chargebacks and fees, and denials of legitimate transactions.

**Understanding and Defining Fraud**
Credit card fraud is any dishonest act and behaviour to obtain information without the proper authorization from the account holder for financial gain. Among different ways of frauds, Skimming is the most common one, which is the way of duplicating of information located on the magnetic strip of the card. Apart from this, the other ways are:

Manipulation/alteration of genuine cards
Creation of counterfeit cards
Stolen/lost credit cards
Fraudulent telemarketing
Data Dictionary
The dataset can be download using this link
https://www.kaggle.com/mlg-ulb/creditcardfraud

The data set includes credit card transactions made by European cardholders over a period of two days in September 2013. Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value 1 in cases of fraud and 0 in others.

**Project Pipeline**
The project pipeline can be briefly summarized in the following four steps:

Data Understanding: Here, we need to load the data and understand the features present in it. This would help us choose the features that we will need for your final model.
Checking the missing values: there was no missing values in the dataset.
Seperating independent an dependent features: we have seperated 1-30 in one set and 31 in other set to diffrentiate the target column.
initialising the target column: we initialise 0 as Not fraud and 1 as Fraud in the other dataset.
we analysing the distribution features of dependent variable and we found it is highly imbalanced approx 99 percent of data lies in a not fraud cases.
then we implement the oversampling method to balanced the dataset.
Train/Test Split: Now we are familiar with the train/test split, which we can perform in order to check the performance of our models with unseen data. Here, for validation.
Model-Building/Hyperparameter Tuning:we can use the models like Logistic Regression,Support Vector Classification,Decision Tree and random Forest model to check teh accuracy.
Model Evaluation: We need to evaluate the models using appropriate evaluation metrics. Note that since the data is imbalanced it is is more important to identify which are fraudulent transactions accurately than the non-fraudulent. We need to choose an appropriate evaluation metric which reflects this business goal.
Finalising the model:So as per model evaluation we find out decision tree model will give the most accurate predication among all , so we deploy that model through pickle file.
