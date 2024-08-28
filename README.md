# **CHURNCOMPASS: NAVIGATING CUSTOMER RETENTION IN TELCOM**
### Project by: Deborah Okeyo
![pexels-joenibraw-1416530](https://github.com/user-attachments/assets/fc1c608d-88c3-407d-88f3-85a35abd52a6)
# 1.Introduction
In today's highly competitive telecommunications industry, customer retention is important for sustained business success. Losing customers (churn), can lead to significant revenue losses, making it essential for telecom companies to proactively identify customers at risk of leaving. This project will focus on developing a predictive model to forecast customer churn by analyzing customer data and identifying key factors that contribute to churn, it will also aim to equip the company with insights to improve customer retention strategies
# 2. Business Problem
The objective of this project is to predict whether a customer will churn (leave the service) in the near future. Accurate churn predictions will allow the company to intervene with targeted retention efforts, potentially saving significant revenue. By understanding the patterns and reasons behind customer churn, the company can gain insights on how to improve their pricing, services, and customer support.

# 3. Data Understanding
The dataset used for this analysis contains customer information, including demographics, account details, and service usage patterns. Key features include tenure, contract type, payment method, monthly charges, and various service-related variables. The target variable is a binary outcome indicating whether the customer has churned or not.

# 4. Exploratory Data Analysis (EDA)
# 4.1 Distribution of Churn

The distribution of the target variable (Churn) shows that there is an imbalance in the dataset, with a higher number of customers not churning compared to those who do. Addressing this imbalance is crucial for building a robust predictive model.

# 4.2 Feature Importance

The Random Forest model's feature importance analysis highlights that tenure, contract type, and monthly charges are the most influential features in predicting customer churn. Features related to the type of services subscribed (like Internet service and tech support) also play a significant role.
![image](https://github.com/user-attachments/assets/57ab2140-e2df-4ba3-88ae-41326df3daf6)

# 5. Data Preprocessing
# 5.1 Handling Missing Values
Missing Values: The dataset had no missing values.
Encoding: Categorical variables were encoded using OneHotEncoding to prepare them for model training.
# 5.2 Addressing Class Imbalance
Given the imbalance in the dataset, we applied the SMOTE (Synthetic Minority Over-sampling Technique) to generate synthetic samples for the minority class (churned customers). This technique helped in building a more balanced and effective predictive model.

# 6. Model Development
# 6.1 Model Selection
A Random Forest Classifier was chosen for its robustness and ability to handle both numerical and categorical data. The model was trained on the preprocessed dataset and evaluated using the test set.

# 6.2 Model Evaluation
The model's performance was evaluated using various metrics:

Accuracy: 78%
Precision (Churn): 63%
Recall (Churn): 45%
F1-Score (Churn): 53%
ROC-AUC: 0.82

# 6.3 Model Performance
The model performed well in predicting non-churned customers but struggled with predicting churned customers accurately. This is reflected in the lower recall and F1-score for the churned class.

# 6.4 ROC Curve

![image](https://github.com/user-attachments/assets/04b3ac7c-91f2-4506-8c0b-16a5e0344557)

The ROC curve shows the model's ability to distinguish between churned and non-churned customers. The AUC (Area Under Curve) of 0.82 suggests a good performance.

# 7. Recommendations
Based on the analysis and model results, the following strategies are recommended to improve customer retention:

Targeting Short-Tenure Customers: Customers with shorter tenures are more likely to churn. Offering them long-term contracts could improve retention.

Re-evaluation of Pricing Strategies: Customers with higher monthly charges are more likely to churn. Consider revising pricing strategies, especially for this segment.

Enhancing Service Offerings: The type of services subscribed (e.g., Internet service) significantly impacts churn. Improving service offerings could reduce churn rates.

Personalizing Retention Efforts: Using the model's predictions, tailor retention strategies to individual customers based on their likelihood to churn.

# 8. Limitations
While the model achieved reasonable accuracy, it struggled with predicting churn accurately, reflected in the low recall rate for churned customers. This limitation suggests that some customers at risk of churning may not be identified by the model. Additionally, potential biases in the dataset, such as demographic or service-related biases, could affect the model's performance.

# 9. Conclusion
This project successfully developed a predictive model to identify customers at risk of churning in the telecom industry. The analysis highlighted key factors influencing churn and provided actionable insights to improve customer retention.

# How to Run the Project
1. Clone the repository to your local machine.

2. Ensure you have the necessary Python libraries installed (pandas, scikit-learn, matplotlib, seaborn).
   
3. Run the notebook file (index.ipynb) to see the full analysis and model training process.

# Project Presentation

[View the project presentation on Canva](https://www.canva.com/design/DAGPCIAAmcQ/EntEME-Hjp27iit7Sj-46w/edit?utm_content=DAGPCIAAmcQ&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

