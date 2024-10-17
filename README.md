# Churn Prediction Model with Random Forest Algorithm and Linear Regression

### Overview:
The primary objective of this project was to develop a predictive model capable of accurately identifying customers at risk of churning. By anticipating customer attrition, businesses can proactively implement strategies to retain valuable customers, reduce churn rates, and improve overall profitability. To achieve this goal, I employed a combination of data analysis, feature engineering, and machine learning techniques.

### DataFrame Structure/Columns
- **RowNumber**—corresponds to the record (row) number and has no effect on the output.
- **CustomerId**—contains random values and has no effect on customer leaving the bank.
- **Surname**—the surname of a customer has no impact on their decision to leave the bank.
- **CreditScore**—can have an effect on customer churn, since a customer with a higher credit score is less likely to leave the bank.
- **Geography**—a customer’s location can affect their decision to leave the bank.
- **Gender**—it’s interesting to explore whether gender plays a role in a customer leaving the bank.
- **Age**—this is certainly relevant, since older customers are less likely to leave their bank than younger ones.
- **Tenure**—refers to the number of years that the customer has been a client of the bank. Normally, older clients are more loyal and less likely to leave a bank.
- **Balance**—also a very good indicator of customer churn, as people with a higher balance in their accounts are less likely to leave the bank compared to those with lower balances.
- **NumOfProducts**—refers to the number of products that a customer has purchased through the bank.
- **HasCrCard**—denotes whether or not a customer has a credit card. This column is also relevant, since people with a credit card are less likely to leave the bank.
- **IsActiveMember**—active customers are less likely to leave the bank.
- **EstimatedSalary**—as with balance, people with lower salaries are more likely to leave the bank compared to those with higher salaries.
- **Exited**—whether or not the customer left the bank.

### Key Findings
- with Random Forest Algorithm, an accuracy of 86% is achieved
- with Linear Regression Model, an accuracy of 81% is achieved
- The attribute, Age, has the highest feature importance
- Random Forest performs better than Regression model

### Methodology
##### 1. EDA
Data source: click [here](https://www.kaggle.com/datasets/mathchi/churn-for-bank-customers/data) <br/>
Conducted exploratory data analysis (EDA) to understand the data distribution, identify missing values, and explore potential relationships between variables.
![](img/output.png)

##### 2. Feature Engineering
- Applying label encoding for binary features
- Normalizing numerical features
- Converting categorical variables (Gender, Geography) into dummy variables
![](img/correlation.png)

##### 3. Model Selection and Training
- Evaluated multiple machine learning algorithms, including random forest and linear regression, to select the most suitable model for churn prediction

##### 4. Model Evalutation
- Random Forest Algorithm has an accuracy of 86%
- Linear Regression Algorithm has an accuracy of 81%

##### 5. Feature Importance
- Analyzed the importance of different features in the model's predictions to identify key drivers of customer churn
![](img/feature_importance.png)
