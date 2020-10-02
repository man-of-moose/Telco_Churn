# Telco_Churn

#### Data Scientists:
- Alec McCabe

#### Sources:
- IBM Customer Retention Dataset, sourced from Kaggle

#### File Guide:

```
'telco_churn' = Data Cleaning and EDA and Hypothesis Testing
'logreg_models' = Multiple Logistic Regressions
' KNN_DTC_RFC' = Multiple Tree, Random Forest, Bag/Boost, etc..
```

## Presentation Link
https://docs.google.com/presentation/d/1G4hcbbq7fX-1cvwU-4ap998n0EXK789XRe8zBRkIajE/edit?usp=sharing

## Introduction

The goal of this project is to provide actionable feedback to a Major Telecom company regarding the optimization / minimization of Customer churn. With this goal in mind, I set out to analyze relevant data in order to better understand the market, and what features lead to an increase chance of a customer churning. From Kaggle, I was able to obtain the IBM Customer Retention Dataset, which includes over 8000 observations pertaining to telecom customers and their respective churn-status.

With this data in hand, my goal is to create an interpretable classification model to assist the Telecom Company in:
```
1. identifying customers who are at-risk of churning
2. identifying which features contribute to churning
3. identifying approaches to mitigate churning
```

In answering the above questions, we utilized the following libraries:

```
### Data Collection and Cleaning
pandas
numpy

### Data Visualization
pandas
matplotplib.pyplot
seaborn

### Statistical Analysis
scipy

### Model Building
sklearn
statsmodels
imblearn

```

## EDA

Dataset consisted of 3 continous and 17 categorical predictors.

##### High Correlation between "Services" features

![Image](pictures/Heatmap.png?raw=true)

#### Certain Features Strongly Correlated with Churn Rate

![Image](pictures/InternetService1.png?raw=true)

![Image](pictures/SeniorCitizen1.png?raw=true)

![Image](pictures/Contract1.png?raw=true)

#### Tenure Strongly Correlated with Churn Rate

![Image](pictures/Tenure_vs_Churn.png?raw=true)

### Best Model: Logistic Regression, Upsampled, Best Features

![Image](pictures/feature_importance_best.png?raw=true)

![Image](pictures/confusion_matrix_best.png?raw=true)


Recommendations:

Upsell Contracts
- 2 Year Contracts contribute the most to prolonged subscription

Fiber Optic Service
- Improve performance of Fiber Optic service to retain customers

Reduce Usge of eChecks:
- Usage of eChecks increases churn rate

Sell Cheap First
- Increase stickiness, slowly. Customers with more tenure will be more willing to accept pricey services

Reduce Paperless Billing
- Usage of Paperless Billing increases change of churn

TechSupport, Online Security
- Lack of TechSupport or OnlineSecurity increases churn - try to sell these services first



## Future Analysis

1. Identify additional data sources to include in the analysis
2. Continue to create new features
3. Additional experimentation with LBGM
