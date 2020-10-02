# Telco_Churn

#### Data Scientists:
- Alec McCabe

#### Sources:
- IBM Customer Retention Dataset, sourced from Kaggle


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


Recommendations:

Competition:
- Investigate the operations of production companies such as Universal Pictures and Warner Brothers to optimize your movie production output 
- Focus on developing large franchises like those owned by Marvel and Lucasfilms in order to maximize total revenue at the box office

Genres:
- Avoid genres like Drama, Comedy, and Thriller as these are highly saturated
- Focus on developing Fantasy, Adventure, and Animation movies as these return the highest profit

Release Month:
- Avoid releasing films in “Dump Months” such as September, as you will have increased competition.

Runtime:
- Based on our analysis, the typical Fantasy, Animation, and Adventure genres are typically 90-100 minutes in duration.



## Future Analysis

1. Retrieve data from social media sources (Twitter, Reddit, Facebook, etc) in order to measure the effectiveness of social media marketing on movie success

2. Retrieve data from online streaming services such as Netflix and Hulu in order to focus on further expansion to online markets

3. Include Production Countries data (from TMDB) in our analysis in order to assist Microsoft in foreign market expansion
