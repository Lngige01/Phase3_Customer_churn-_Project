**PHASE 3 PROJECT**


**SYRIATEL CUSTOMER CHURN**

*Student: Lilian Ngige*

**Project Overview**

The project aims at analysing SyriaTel data and building models that predict whether a customer will churn or not.

**Business Problem**
SyriaTel, a telecommunications company, is facing the challenge of customer churn. The company wants to predict whether a customer is likely to stop doing business with them in the near future. Reducing customer churn is essential for maintaining revenue and profitability.

**Project Objective**
Build a binary classification model to predict customer churn. The model will identify customers who are likely to churn, to enable SyriaTel to take proactive measures to retain them.

**Stake holder audience**
The stake holder is the Telecomunication share holders

**The Data**
This dataset has 3,333rows and 21 columns. We shall use this data for predicting customer churn, which is crucial for the telecommunication company to understand and reduce customer attrition. We shall employ the date to develop predictive models to identify customers at risk of leaving the service and implement retention strategies to reduce churn.

**Exploratory data analysis**
#Bar graph to show distribution of the target variable "churn'


**Data preparation for Machine Learning**

Correlation coeffient: The colleration of features to the target variable
Train-test split: Data is split into train and test sets.
Transform categorical variables: dummy variables are created for categorical features.
SMOTE: SMOTE is used to handle class imbalance problems by oversampling the minority class with replacement.

**Modelling**
we use three models to train and test the data and check the performance.
The first model I use is baseline model that is the logistic regression
**Logistic Regression Results:**
Logistic Regression Results:
Accuracy: 0.71
Classification Report:
               precision    recall  f1-score   support

       False       0.69      0.70      0.70       687
        True       0.72      0.71      0.71       738

    accuracy                           0.71      1425
   macro avg       0.70      0.71      0.71      1425
weighted avg       0.71      0.71      0.71      1425

The second model is **Random forest**

**Random Forest Results:**
Random Forest Results:
Accuracy: 0.96
Classification Report:
               precision    recall  f1-score   support

       False       0.95      0.97      0.96       687
        True       0.97      0.96      0.96       738

    accuracy                           0.96      1425
   macro avg       0.96      0.96      0.96      1425
weighted avg       0.96      0.96      0.96      1425

**The third Model**
Model with Hyperparameter Tuning (Decision tree)
Best Hyperparameters: {'max_depth': 10, 'min_samples_split': 2}
Accuracy: 0.9192982456140351
Classification Report:
               precision    recall  f1-score   support

       False       0.89      0.96      0.92       687
        True       0.96      0.88      0.92       738

    accuracy                           0.92      1425
   macro avg       0.92      0.92      0.92      1425
weighted avg       0.92      0.92      0.92      1425





**Model Evaluation and Comparison**
The performance of the three models
Best-performing model in terms of accuracy and other three metrics(precision,recall & f1 score).


**Conclusions and recommendations**

The metrics indicate that the churn prediction models are performing commendably, with Random Forest emerging as the top performer, boasting an accuracy of 97% and a recall of 96%. Considering the provided test metrics, the Random Forest model appears to outperform the other models in terms of accuracy, precision, recall, and F1-score. It achieves the highest test accuracy, precision, and F1-score, as well as a high test recall. This suggests that the Random Forest model is effective in making accurate predictions with a good balance between precision and recall.

Overall, the high-performing model can help the telecom company proactively address customer churn, potentially saving revenue and improving customer satisfaction

Recommendation

Churn Analysis • Regularly review churn data to identify patterns, reasons, and trends to make more informed decisions.

**Next Step**
Customer retention is an ongoing process, and strategies should evolve based on changing customer behaviors and market dynamics. The insights from the model serve as a valuable foundation for developing and fine-tuning your customer retention initiatives.

Feature engineering: Create new relevant features or transform existing ones to provide better information to the model.
