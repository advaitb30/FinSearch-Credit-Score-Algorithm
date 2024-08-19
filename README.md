# FinSearch-Credit-Score-Algorithm
Objective: We will be creating a model to predict a suitable Credit Score given various features of each borrower.

About Dataset:
The dataset comprises information on 1000 customers, with 84 features derived from their financial transactions and current financial standing. The primary objective is to leverage this dataset for credit risk estimation and predicting potential defaults.

CUST_ID: Unique customer identifier
Key Target Variables:

CREDIT_SCORE: Numerical target variable representing the customer's credit score (integer)
DEFAULT: Binary target variable indicating if the customer has defaulted (1) or not (0)
Description of Features:

INCOME: Total income in the last 12 months
SAVINGS: Total savings in the last 12 months
DEBT: Total existing debt
R_SAVINGS_INCOME: Ratio of savings to income
R_DEBT_INCOME: Ratio of debt to income
R_DEBT_SAVINGS: Ratio of debt to savings
Transaction groups (GROCERIES, CLOTHING, HOUSING, EDUCATION, HEALTH, TRAVEL, ENTERTAINMENT, GAMBLING, UTILITIES, TAX, FINES) are categorized.

T_{GROUP}_6: Total expenditure in that group in the last 6 months
T_GROUP_12: Total expenditure in that group in the last 12 months
R_[GROUP]: Ratio of T_[GROUP]6 to T[GROUP]_12
R_[GROUP]INCOME: Ratio of T[GROUP]_12 to INCOME
R_[GROUP]SAVINGS: Ratio of T[GROUP]_12 to SAVINGS
R_[GROUP]DEBT: Ratio of T[GROUP]_12 to DEBT
Categorical Features:

CAT_GAMBLING: Gambling category (none, low, high)
CAT_DEBT: 1 if the customer has debt; 0 otherwise
CAT_CREDIT_CARD: 1 if the customer has a credit card; 0 otherwise
CAT_MORTGAGE: 1 if the customer has a mortgage; 0 otherwise
CAT_SAVINGS_ACCOUNT: 1 if the customer has a savings account; 0 otherwise
CAT_DEPENDENTS: 1 if the customer has any dependents; 0 otherwise

About the model:
We will use Random Forest Regressor from "sci-kit learn" library of python as it provides accurate results and is a more convenient option.
GridSearch along with RandomForestRegressor helps increase the accuracy by selecting the best set of parameters.

