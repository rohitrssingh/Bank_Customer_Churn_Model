# Bank_Customer_Churn_Model

Learning Objective:

The goal of this project is to predict whether a customer is likely to churn (leave the bank) using a machine learning approach. This model addresses various important steps, including data preprocessing, handling imbalanced data, and model optimization, as outlined below:

1. Data Encoding:
   
Since the dataset contains categorical variables (such as customer gender or geographic region), encoding techniques are applied to convert these non-numeric values into numeric ones. Methods like One-Hot Encoding or Label Encoding are used to make the data suitable for machine learning models.

2. Feature Scaling:
   
Different features in the dataset may have different scales (e.g., age vs. account balance). To ensure that all features contribute equally to the model, feature scaling techniques such as StandardScaler or MinMaxScaler are applied. This helps avoid bias in models like Support Vector Machines (SVM), which are sensitive to the magnitude of the input features.

3. Handling Imbalanced Data:
 
Customer churn datasets are often imbalanced, meaning that the number of customers who churn is much smaller than those who don't. This can bias the model toward predicting non-churn. To address this, we apply techniques such as:

3(a). Random Under Sampling: Reducing the number of majority class samples to balance the dataset, though this may lead to loss of valuable information.

3(b). Random Over Sampling: Increasing the number of minority class samples by duplicating them, which helps balance the dataset but could lead to overfitting.


4. Support Vector Machine (SVM) Classifier:
 
An SVM is used to classify whether a customer will churn or not. This algorithm works by finding the hyperplane that best separates the churners from non-churners in the feature space. It's particularly effective for complex, high-dimensional datasets.


5. Grid Search for Hyperparameter Tuning:
    
To improve model performance, Grid Search is applied for hyperparameter tuning. This process systematically tests various combinations of hyperparameters (such as kernel types, C-values, and gamma) to find the optimal configuration for the SVM model. Hyperparameter tuning ensures that the model performs at its best without overfitting or underfitting.


Conclusion:

By following these steps, we develop a robust model that can accurately predict customer churn. With proper data preprocessing, handling imbalance, and optimizing the SVM classifier, the model provides actionable insights to banks for retaining at-risk customers.
