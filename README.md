# Loan-approval-prediction-using-ML
## Outcome of the Project:- People with the best credit and a co-applicant are more likely to get approved for a large loan.


## Table of Contents
- [Problem Statement](#problem-statement)
- [Data Source](#data-source)
- [Steps](#steps)
- [Tech Stack](#tech-stack)
- [Results](#results)
- [Lessons Learned and Recommendations](#lessons-learned-and-recommendations)

## Problem Statement
This model forecasts the loan amount an applicant will receive. Based on various profile details, the model predicts how much will be permitted. Factors such as a higher credit score in a co-applicant typically lead to a larger loan amount, as well as the amount requested by the applicant.

## Data Source
The data used for this project comes from the [Kaggle Loan Amount Prediction dataset](https://www.kaggle.com/), which includes various applicant features to aid in predicting loan amounts.

## Steps
1. **Exploratory Data Analysis**
2. **Bivariate Analysis**
3. **Multivariate Correlation Analysis**

## Tech Stack
- **Python** 

## Results
The top 3 models (using default parameters) and their performance are as follows:

| Model with the best hyperparameter| RMSE (Range: 0 - 400,000) |
|---------------------|---------------------------|
| Random Forest       | 20,784.89                 |
| Bagging             | 20,723.30                 |
| Gradient Boosting   | 26,674.35                 |

-_ **Final Model Used**: Random Forest
- **Metric Used**: RMSE (Root Mean Squared Error)_

**Why choose Random Forest while Bagging yields the best results?**  
Although Bagging produced the lowest RMSE, Random Forest was selected because it consistently produced the lowest RMSE during parameter tuning.

## Lessons Learned and Recommendations
Through this project, we found that the primary factors influencing the loan amount granted are:
- The requested loan amount
- The applicant's credit score
- Presence of a co-applicant

Features with minimal impact include:
- Expense types
- Gender

**Recommendation**: Focus on the most predictive features when reviewing applicant profiles, while placing less emphasis on the least predictive features.
