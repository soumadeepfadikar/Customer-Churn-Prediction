 Customer Churn Prediction - Final Report

 1. Introduction
Customer churn refers to customers discontinuing their relationship with a business. This project aims to predict customer churn using machine learning models, enabling businesses to retain at-risk customers by taking proactive measures.

 2. Dataset Information
The dataset includes customer demographic, account, and service-related attributes. The target variable, **Churn**, indicates whether a customer has left the service.

 Key Features:
- **Demographics**: Gender, Senior Citizen status, etc.
- **Account Information**: Tenure, Monthly Charges, Total Charges
- **Services Used**: Internet Service, Streaming, Security Features, etc.

 3. Data Preprocessing
- **Handling Missing Values**: Imputed missing values in Total Charges with median.
- **Encoding Categorical Variables**: Applied Label Encoding for binary variables and One-Hot Encoding for categorical variables.
- **Feature Scaling**: Standardized numerical features to improve model performance.
- **Train-Test Split**: 80% training and 20% testing data.

 4. Model Training and Evaluation
We implemented the following models:

 4.1 Logistic Regression
- Baseline model for churn prediction.
- Achieved an **accuracy of 79%**.

 4.2 Random Forest Classifier
- More complex model for better accuracy.
- Achieved an **accuracy of 82%**.

 4.3 Hyperparameter Tuning
- Performed GridSearchCV on Random Forest.
- Best model achieved an **accuracy of 84%**.

 5. Model Performance Metrics
| Model                   | Accuracy | Precision | Recall | F1-score |
|-------------------------|----------|-----------|--------|-----------|
| Logistic Regression     | 79%      | 0.74      | 0.65   | 0.69      |
| Random Forest          | 82%      | 0.78      | 0.70   | 0.74      |
| Tuned Random Forest    | 84%      | 0.80      | 0.72   | 0.76      |

 6. Business Impact
- The model helps identify customers at risk of churning.
- Businesses can implement targeted retention strategies.
- Reducing churn increases customer lifetime value and revenue.

 7. Conclusion
This project successfully developed a machine learning model to predict customer churn. The **tuned Random Forest model** performed the best, providing valuable insights for customer retention strategies.

 8. Future Work
- Explore deep learning techniques for improved accuracy.
- Use additional customer interaction data for better insights.
- Implement real-time prediction in a production environment.

