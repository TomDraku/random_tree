Project Overview

This project, undertaken as part of the Python for Data Science and Machine Learning Booamp course, explores the use of Random Forests for predicting loan defaults on LendingClub.com data. The goal is to develop a model that can assess a borrower's creditworthiness and determine the likelihood of them repaying a loan in full.

Data Description

This project utilizes LendingClub.com loan data from 2007-2010, focusing on predicting whether a borrower defaulted on their loan. The provided CSV dataset (cleaned of NA values) consists of the following features:

credit.policy: Binary (1/0) indicating adherence to LendingClub's credit standards.
purpose: Loan purpose category ("credit_card", "debt_consolidation", etc.).
int.rate: Interest rate of the loan as a proportion (e.g., 0.11 for 11%).
installment: Monthly loan installment amount.
log.annual.inc: Natural logarithm of the borrower's self-reported annual income.
dti: Borrower's debt-to-income ratio.
fico: Borrower's FICO credit score.
days.with.cr.line: Number of days with a credit line.
revol.bal: Borrower's revolving credit card balance.
revol.util: Borrower's credit line utilization rate.
inq.last.6mths: Number of credit inquiries in the last 6 months.
delinq.2yrs: Number of 30+ day past-due payments in the last 2 years.
pub.rec: Number of derogatory public records (bankruptcy, tax liens, judgments).
Target Variable

The target variable in this dataset is binary, indicating whether a borrower defaulted on their loan or not (represented as a boolean value).

Project Steps

Data Loading and Exploration:
Import necessary libraries (e.g., pandas, NumPy, scikit-learn).
Load the CSV data into a pandas DataFrame.
Explore the data through:
Descriptive statistics for numerical features.
Frequency tables for categorical features.
Data visualization techniques (histograms, boxplots, etc.) to examine distributions and relationships.
Data Preprocessing:
Address missing values (if any, but the provided dataset should be clean).
Encode categorical features using techniques like one-hot encoding.
Perform feature scaling or normalization if necessary.
Model Building:
Split the data into training and testing sets.
Create a Random Forest classifier instance, specifying hyperparameters like the number of trees (n_estimators).
Fit the model to the training data.
Model Evaluation:
Evaluate model performance on the testing set using metrics like accuracy, precision, recall, F1-score, and AUC-ROC.
Consider hyperparameter tuning to improve model performance if needed (e.g., using GridSearchCV).
Results and Interpretation:
Report the model's performance metrics.
Analyze the importance of features in predicting loan defaults using the Random Forest's built-in feature importance scoring.
Discuss the project's findings and potential limitations.
Project Dependencies

Python 3.x
pandas
NumPy
scikit-learn (specifically RandomForestClassifier, metrics, etc.)
Additional Notes

Consider using data visualization libraries like Matplotlib or Seaborn to create informative plots.
Explore feature engineering techniques that might create new features for improved model performance.
Document your code clearly and consistently using comments and docstrings.
Feel free to adapt these steps and explore other aspects of machine learning or data science that interest you within this project context.
