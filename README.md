# Home Credit Default Risk Analysis

## Overview
The [**Home Credit Default Risk Analysis**](https://www.kaggle.com/competitions/home-credit-default-risk) project aims to enhance financial inclusion by predicting loan repayment capabilities for individuals with limited or no credit history. Using alternative data, we developed a supervised machine learning model to evaluate creditworthiness and provide actionable insights for lenders.

## Business Problem
Financial institutions often rely on traditional credit scores, which can exclude individuals lacking credit history. This project focuses on creating a predictive model that utilizes alternative data sources, enabling informed lending decisions and expanding opportunities for both borrowers and lenders.

## Objectives
- Develop a predictive model to evaluate loan default risk.
- Increase loan approval rates while maintaining or reducing lender risk.
- Provide business insights to drive data-informed decision-making.

## Data and Methodology
- **Data Sources:** Provided datasets include demographic, transactional, and telco data from orignial [Kaggle](https://www.kaggle.com/c/home-credit-default-risk/overview) competition 
- **EDA:** Explored trends, identified missing values, and performed data preprocessing.
- **Feature Engineering:** Created new variables to enhance predictive performance.
- **Modeling:** Built and fine-tuned a logistic regression classifier to predict loan defaults.
- **Visualization:** Generated insightful plots to communicate findings effectively.

## Key Contributions
This notebook includes:
- [**Exploratory Data Analysis (EDA):**](https://github.com/leemr0903/HomeCredit/blob/1842ce94ad9df862efa3115aa393a1138f51f95a/MSBA_Practice_EDA_Revised.Rmd) Analysis of key patterns and trends in the data.
- **Feature Engineering:** Detailed feature transformations to improve model accuracy.
- [**Individual Model Development:**](https://github.com/leemr0903/HomeCredit/blob/1842ce94ad9df862efa3115aa393a1138f51f95a/MSBA_Practice_Modeling_Assignment.Rmd) Training and evaluation of the predictive model.
- [**Final Group Model:**](https://github.com/leemr0903/HomeCredit/blob/cd6ce098af301af94f56342769b62df152a99f30/Group%201%20Modeling%20Notebook%20-%20Whitney%20Holt%2C%20Maddie%20Lee%2C%20Alexia%20Wells%2C%20Leah%20Ekblad.Rmd) Collaborative development of the final predictive model, integrating insights and refinements from individual contributions.
- **Results Interpretation:** Business value insights derived from the analysis.
- [**Business Presentation Slides:**](https://github.com/leemr0903/HomeCredit/blob/aec3e9fb9df15415f07db1a5347777ce875380a5/Enhancing%20Loan%20Approval%20Processes%20through%20Predictive%20Modeling%20-%20Capstone%20Project.pptx) Summarized key findings and recommendations in a stakeholder-friendly format, highlighting the model's impact on financial inclusion.

## Indiviual Contributions

## Challenges 

### 1. Missing Values
- Many features contain missing values, which can introduce bias if not handled properly.  
- Missing values may represent a lack of information, errors in data entry, or genuine absence of certain attributes.  
- Imputation techniques must be carefully chosen to avoid distorting the underlying patterns in the data.  

### 2. High Cardinality
- Certain categorical variables, such as occupation type or income type, have numerous unique values.  
- High cardinality increases model complexity and can lead to overfitting, especially when one-hot encoding is applied without adequate dimensionality reduction.  

### 3. Imbalanced Target Variable
- The target variable (loan default) is heavily imbalanced, with significantly more non-default than default cases.  
- This imbalance can bias models toward predicting the majority class, reducing their ability to identify true default risks.  

### 4. Inconsistent Factor Levels
- Some categorical variables contain levels present in one dataset but missing in another (e.g., `NAME_INCOME_TYPE`).  
- This inconsistency complicates model application across datasets and requires alignment of factor levels or handling of unknown levels.  

### 5. Collinearity Among Features
- Certain features, such as income and credit amount, are highly correlated, leading to multicollinearity in linear models.  
- Multicollinearity inflates the variance of coefficient estimates, making the model sensitive to small changes in the data and potentially reducing interpretability.  

### 6. Outliers and Noise
- Some numerical features contain extreme values that may be outliers or data entry errors.  
- These values can distort model training, especially in distance-based or sensitive algorithms, necessitating careful inspection and possible transformation or filtering.  

### 7. Large Dataset and Load Times
- The size of the dataset significantly impacts processing time.  
- Loading and training on just 5% of the data can take over an hour, limiting experimentation.  
- Optimized workflows, hardware improvements, or data subsampling may be necessary to address this challenge.


## Learnings
  
## Business Impact
By leveraging this model, lenders can:
- Approve more loans for individuals with limited credit history.
- Enhance profitability by reducing default rates and expanding the client base.
- Support financial inclusion initiatives for underserved populations.

