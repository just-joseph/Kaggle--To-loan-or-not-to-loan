# Kaggle--To-loan-or-not-to-loan

Problem description:
https://www.kaggle.com/c/to-loan-or-not-to-loan


Problem approach:
1. Factor mapping
2. Finding correlations or dependencies between variables and with output variable (loan status)
2. Model to predict if an existing loan would default. (OBJ1_model1)
3. Model to predict if a new loan can be granted to an existing customer. (OBJ2_model2)
4. Use AutoML (Tpot, H2O, Google AutoML etc) for better modelling.
5. Identify cross selling strategies
6. Future Scope

Data from 1993 to 1998.
Data proprocessing:
Dates were converted to ages (compared to 1999).
Gender identified.

Data split to train and test. 
Random forests- High accuracy with high precision & recall. 
Features which influenced the model the most were identified- they were mostly attributes of bank or customer and not transaction data.

Future scope:
1. Aggregation of transaction data on different timeframes (monthly, quarterly, half yearly, yearly etc) to derive more insights.
2. OBJ1 (Model 1) has a major flaw- 
the train data should only have data till the time before defaulting (Like how OBJ2 data had only data upto the month being granted the loan). We need to correct this. 
3. Derive more business related insights (in terms of finance)
4. Use ROC curve and AUC value to identify best model and compare with AutoML output.
