# Classification Project
This repo is for demonstration and display of my telco classification project

# About the Project
## Project Goals
The goal of this project is to identify key drivers of churn at Telco and develop a model to accurately predict 
customer churn-- as well as deliver my findings appropriately in addition to making recommendations on how to set 
up customers for retention.

## Project Description
It is less expensive to retain customers than it is to find new ones. In this project, we will analyze the attributes of 
customers who churn and devlop a model to predict customer churn. Deliverables are recommendations for companies with churning customers
and predictions for new customers.

## Initial Questioins
Where is the churn?

Why are these customers churning?

1. What percentage of customers are churning overall? For the 1 year plan? The 2 year plan? The month-to-month plan?

2. Do churned customers have higher average charges than retained customers? Are higher charges associated with churn? 

3. What is the churn rate for male customers vs female customers?

4. What is the rate of churn for customers with dependents vs customers without?

5. Is there any difference in churn rate for customers with a partner vs customers without?

6. Are customers with a certain subscription more likely to churn?

## Data Dictionary
 | Feature                     | Datatype                | Description                                                                                  |
 |:----------------------------|:------------------------|:---------------------------------------------------------------------------------------------|
 | customer_id                 | index (object)          | Alpha-numeric ID unique to each customer                                                     |
 | is_male                     | 7043 non-null: uint8    | Customer gender. 0: Female / 1: Male                                                         |
 | senior_citizen              | 7043 non-null: int64    | Senior citizen status. 0: Not a senior / 1: Senior                                           |
 | partner                     | 7043 non-null: int64    | Partner status. 0: No partner  / 1: Has partner                                              |
 | dependents                  | 7043 non-null: int64    | Dependent status. 0: No dependents  / 1: Has dependents                                      |
 | phone_service               | 7043 non-null: int64    | Phone service status. 0: No phone service / 1: Has phone service                             |
 | paperless_billing           | 7043 non-null: int64    | Paperless billing status. 0: No / 1: Yes                                                     |
 | churn                       | 7043 non-null: int64    | Churn status. 0: No / 1: Yes                                                                 |
 | tenure                      | 7043 non-null: int64    | Number of months a customer has been with Telco                                              |
 | monthly_charges             | 7043 non-null: float64  | Monthly charges for each customer                                                            |
 | total_charges               | 7043 non-null: float64  | Total charges for each customer                                                              |
 | multiple_lines              | 7043 non-null: uint8    | Multiple lines status. 0: No / 1: Yes                                                        |
 | online_security             | 7043 non-null: uint8    | Online security status. 0: No / 1: Yes                                                       |
 | online_backup               | 7043 non-null: uint8    | Online backup status. 0: No / 1: Yes                                                         |
 | device_protection           | 7043 non-null: uint8    | Device protection status. 0: No / 1: Yes                                                     |
 | tech_support                | 7043 non-null: uint8    | Tech support status. 0: No / 1: Yes                                                          |  
 | streaming_tv                | 7043 non-null: uint8    | Streaming TV status. 0: No / 1: Yes                                                          |
 | streaming_movies            | 7043 non-null: uint8    | Streaming movies status. 0: No / 1: Yes                                                      |
 | m2m_contract                | 7043 non-null: uint8    | Month-to-month contract status. 0: No / 1: Yes                                               |
 | one_year_contract           | 7043 non-null: uint8    | One-year contract status. 0: No / 1: Yes                                                     |
 | two_year_contract           | 7043 non-null: uint8    | Two-year contract status. 0: No / 1: Yes                                                     |
 | DSL_internet                | 7043 non-null: uint8    | DSL internet status. 0: No / 1: Yes                                                          |
 | Fiber_internet              | 7043 non-null: uint8    | Fiber_internet status. 0: No / 1: Yes                                                        |
 | no_internet                 | 7043 non-null: uint8    | Internet service status. 0: Yes / 1: No                                                      |
 | bank_auto_payment           | 7043 non-null: uint8    | Automatic bank payments status. 0: No / 1: Yes                                               |
 | card_auto_payment           | 7043 non-null: uint8    | Automatic credit card payments status. 0: No / 1: Yes                                        |
 | electronic_check_payment    | 7043 non-null: uint8    | Electronic check payments status. 0: No / 1: Yes                                             |
 | mailed_check_payment        | 7043 non-null: uint8    | Mailed check payments status. 0: No / 1: Yes                                                 |
 | high_charges                | 7043 non-null: bool     | Indicates whether or not customer monthly charges are high. True or False                    |
 | higher_than_average_charges | 7043 non-null: bool     | Indicates whether or not the customer monthly charges are higher than average. True or False |

## Steps to Reproduce
Clone this repository and copy personal env.py into repo to run (personal valid credentials necessary).
Libraries used are pandas, numpy, matplotlib, seaborn and sklearn.

## The Plan
### Wrangle
-Write modules with functions that acquire, prepare and split the data.
-Import modules into notebook and test functions
-Document individual reasons for data prep

### Explore
-explore through visualizations and statistical testing
-summarize findings

### Modeling
#### Select evaluation metric
-clearly explain how models were evaluated and compared
-what metrics did I use and why?
#### Evaluate baseline
#### Develop 3 models
#### Evaluate on train
#### Evaluate on validate 
#### Evaluate top model on test

### Report
-thoroughly commented code
-markdown thought processes, decisions, and navigations through the pipeline
-leave no doubt as to why you did something; keep it simple

#### Written conclusion summary
-address questions raised in opening
-summary should tie together analysis, drivers of outcome, and expectations on future unseen data in layman's terms

#### conclusion (recommendations)
-ending conclusion should contain actionable recommendations based on your insights and analysis to the simulated audience

#### conclusion (next steps)
-next steps from a data science perspective (assist in improving future research)
