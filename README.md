# Credit Risk Scorecard & Expected Loss Modeling

## Business Context
When a bank receives a loan application, it must assess the risk of the applicant defaulting. 
Approving too many risky applicants increases credit losses. 
Rejecting too many good applicants reduces revenue. 
This project builds a credit risk model that quantifies this trade-off and translates it into actual financial impact.

## Dataset
Personal loan data with 32,581 applicants and 12 features, including loan 
amount, income, employment length, loan grade, and credit history.

## What I Built
1. **Data Cleaning**: removed outliers and handled missing values
2. **Logistic Regression**: baseline model, ROC-AUC: 0.763
3. **XGBoost**: improved model with feature importance analysis, ROC-AUC: 0.946
4. **Acceptance Rate Analysis**: shows how the default rate changes at different approval thresholds
5. **Expected Loss Calculation**: quantifies money saved by using the model vs approving everyone

## Key Finding
By approving only the safest 50% of applicants, the model reduces the 
default rate from 21.82% down to ~3%, saving the bank **$6,351,791** 
in expected losses compared to approving everyone with no model.

## Tools
Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn
