# Credit-Risk-Analytics
The business objective is building a predictive model to estimate the likelihood of loan defaults, and categorize borrowers into risky or safe classifi cations, and identifying the signifi cant variables impacting default probability, to enable proactive risk management. The project is framed as a classifi cation task, with loan status as the target variable. Predictor variables include demographics, loan characteristics, credit history, and employment details. The scope covers the complete ETL process, including exploratory data analysis (EDA), data cleaning and transformation, model development, evaluation, deployment on the model into clients’ loan approval systems, and feedback and monitoring. This platform proposal will assist institutions evaluate risk more accurately and restructure their lending frameworks accordingly to reduce their default rate by identifying low-risk applications, hence improving financial security, profi tability and compliance with credit risk management regulations.
## Model Selection: Random Forest for Credit Risk Prediction
When building a predictive model for credit risk, it is imperative to evaluate and compare the various machine learning models and identify the best fi t for the dataset. In this case, Random Forest was chosen over simpler models like Logistic Regression, Linear Regression, and standalone Decision Trees, primarily due to the skewed nature of the dataset and its superior handling of non-linearity and relationship complexities.

<b>Why Random Forest Is the Best Choice</b>
1. Robustness to Skewed Data

As an ensemble learning method, Random Forest combines multiple Decision Trees, making it particularly immune to imbalanced datasets. Its process of subsetting and aggregating results allows it to tackle imbalance, missing values and outliers. Alternate models such as logistic regression use the log-odds of the target variable, making them vulnerable to an imbalanced class, and require explicit preprocessing to manage missing data and outliers. Decision Trees often overfi t skewed data by focusing excessively on minimizing impurity without accounting for imbalance.

2. Non-Linear Relationships and Feature Interactions

The Credit risk dataset has complex, non-linear relationships and interactions between its different features, such as income, employment length, and loan amount. Random Forest captures these complexities by learning unique aspects of the data, and modeling the nonlinear interactions. Linear Regression on the other hand, produces overly simplistic outcomes resulting in low performance. Random Forest amplifi es the capabilities of decision trees and overcomes its structural limitations to deliver comprehensive insights.

3. Overfitting Prevention

Random Forest incorporates such as bootstrap aggregation to tackle overfi tting. Each tree is trained on a random subset of the data, and random subsets of features are used to split nodes. These techniques introduce randomness, ensuring that the model generalizes well to new, unseen data. In contrast, a single Decision Tree is highly prone to overfi tting as it seeks to perfectly classify the whole training data. Logistic Regression, while less prone to overfi tting, lacks the versatility to capture complex, non-linear patterns in data.

4. Feature Importance

Random Forest reliably develops a feature importance measure to identify the most impactful predictors. This capability is especially valuable in credit risk applications, where interpretability is essential for meeting regulatory and business requirements. Logistic Regression and Decision Trees indicate variable importance but struggle with non-linearity and overfi tting, while Random Forest overcomes these obstacles to provide a more reliable and insightful feature importance score.
