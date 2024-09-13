# Modeling-Hospital-Length-of-Stay-with-Linear-Regression
Modeling Hospital Length of Stay with Linear Regression

Course: GPH-GU 2353: Linear Regression and Modeling
Contributors:
Varun Putta
Mark Bond
Shahzaib Shaikh
Behrooz Nasir
Introduction
This study aims to develop a reliable method for estimating the duration of hospital stays for patients, which is crucial for effective patient care planning and hospital resource management. We utilize a dataset from Kaggle containing visit-level information on 100,000 patients admitted to hospitals. The main outcome variable is "Length of Stay" (LOS), defined as the number of days a patient spends in the hospital.

The analysis incorporates various additional variables, including:

Disease status (e.g., asthma, iron deficiency)
Levels of health biomarkers (e.g., hematocrit, glucose)
Readmission frequency within the last six months
Irrelevant variables, such as patient and hospital identifiers, were removed to enhance the analysis's focus and clarity.

Data Analysis
Univariate Analysis: Categorical and continuous variables were analyzed to ensure data integrity and relevance.
Unadjusted Model: The initial model included all variables to determine their influence on LOS, revealing a limited R-squared value of 0.18, indicating modest predictive power.
Testing Assumptions: Residuals were analyzed for non-linearity and potential outliers, using Q-Q plots and histograms to assess normality.
Model Adjustment
To address non-linearity and outliers:

Transformations: Box-Cox and log transformations were explored, along with polynomial transformations for predictor variables.
Outlier Assessment: Studentized residuals were calculated, and while many outliers were identified, they were retained in the final model due to negligible changes in R-squared.
Model Selection
The model selection process employed Bayesian Information Criterion (BIC) to identify the optimal model. The final model, incorporating significant predictors, demonstrated an adjusted R-squared value of 0.1446, highlighting the role of categorical variables like end-stage renal disease and psychological disorders.

Summary
This study leverages a large dataset to explore the impact of health conditions on hospital length of stay. Despite challenges in predictive power and model assumptions, the findings underscore key predictors and suggest pathways for future research. Enhancing model accuracy through addressing identified limitations remains a priority for subsequent studies.

Next Steps
Feature Engineering: Introduce new interaction terms and transformations to enhance model accuracy.
Data Augmentation: Integrate additional socio-economic and environmental data.
Collaborative Ethical Framework: Work with healthcare professionals to ensure clinical relevance and address biases in socio-economic variables.
References
For more details and access to the code, please refer to the project files in this repository.
