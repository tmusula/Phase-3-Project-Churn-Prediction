# Churn Analysis for SyriaTel
 
This project uses predictive modeling classification and data visualization to examine customer churn at SyriaTel, a telecommunication company. The objective is to identify patterns in customer behavior and build and evaluate the best model to forecast churn.

# Contents
## 1. Business Understanding
In the telecommunications industry, churn refers to the number of customers who were previously active but are no longer using the company's services. A lot of effort and resources are used to acquire customers, and therefore, it is necessary to ensure that the customers stay with the company for as long as possible.

The objective of this project is to develop a predictive model to identify customers likely to churn, enabling proactive intervention.

## 2. Data Understanding
The dataset consists of 3,333 rows and 21 columns and contains both categorical and numerical variables
The target variable is churn (Boolean), checking whether the customer churned (True/False). Customer demographics data includes account length, phone number etc.
Usage data includes daytime calls, evening calls, nighttime calls, and international calls and customer service data includes customer service calls, and customer support interactions.

## 3. Data Cleaning
Data Cleaning is necessary to prepare the data for analysis and modeling. The data cleaning actions taken include;
- Removed duplicates and missing values (no duplicates or missing data)   
- Dropped irrelevant columns (e.g., phone number, area code).      
- Converted categorical variables to numeric (e.g., international plan: Yes = 1, No = 0).      
- Addressed class imbalance with SMOTE. 
The outcome of the cleaning exercise was a clean data set with 18 features.

## 4. Data Reprocessing
The data reprocessing actions taken included;
 - Handling Missing Values- missing values were identified and imputed using mean/mode techniques where appropriate.
- Feature Encoding - categorical variables were encoded using one-hot encoding.
- Feature Scaling - numerical features were standardized to improve model performance.





## 5. Exploratory Data Analysis (EDA)
Key observations from the dataset include;
(a) Detection of outliers - detecting outliers in numerical features, helping visualize data distribution and identification of the extreme values that could impact analysis or modeling.



## 6. Modeling
The following models have been developed to forecast the likelihood of churn-:
- Logistic Regression
- Random Forest
- Gradient Boosting

The models have been evaluated against the following metrics:
- Accuracy
- Precision, Recall, F1-Score
- ROC-AUC Curve
  
## 7. Model Evaluation
From the results of the metrics, the Random Forest model achieved the highest accuracy at 100%.

The key predictors of churn have been identified as;
- Call usage patterns (minutes and international calls)
- Subscription plans (international plan)
  
## 8. Conclusion and Recommendation
### Conclusion
- Random Forest is the model with the best level of churn prediction out of the evaluated models.
- The variables driving churn have been identified
- The model can enable data-driven decision-making and interventions across the business to manage churn.

### Recommendation
The following actions have been recommended to SyriaTel from the project
- Monitoring of usage patterns to identify customers with unusually high daytime call minutes and assess their satisfaction levels through surveys or feedback channels.
- As part of driving loyalty, introduce daytime offers to provide special discounts or loyalty rewards for high daytime callers to increase satisfaction and loyalty.
- Explore the option of optimizing pricing plans to allow more callers during off-peak hours.
- Offer competitive international calling plans.
- Launch a loyalty program targeting frequent international callers. 
- Monitor the quality of calls for international calls to ensure service disruption doesn't occur. 
- Provide tiered pricing plans or rewards based on call volume to incentivize continued usage.
- Offer loyalty rewards or exclusive perks to customers who have been with the company for a significant period.
- Proactively anticipate churn - monitor behavior changes in long-term customers (e.g., reduced usage) as early indicators of potential churn.
- Ensure customer service issues are resolved effectively during the first interaction.

## 9. Reference
- Dataset Source: *(https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset).
- Libraries Used: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
