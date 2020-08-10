# Bank-Customer-churn-prediction

**Motivation:**

Customer churn is a very important metrics for company to measure their products. Predicting customers churn can help the company know future behaviors of their customers and then can take actions to improve the outcome.

In this project, logitics regression, random forest and LightGBM models were used to predict the customer churn and hyperparameters were tuned to get the best model.


**Step1: Data exploratory analysis**
* Find the percentage of exited customers
* Generated plots to see the distributions of features in exited group and not exited group
* Caculated the correlation between features

**Step2: Feature preprocessing**
* Did one hot encoding to categorical features 
* Split data into trainning set and testing set
* Data standarization on trainning set

**Step3: Trained LR, RF and LGBM models and tune the hyperparameters**
* LR: l1 and l2 regularization
* RF and LGBM: number of trees

**Step4: Model evalution** 
* Generated confusion matrix to see the performance of three models
* Drawd ROC AUC curve
* Feature importance of RF and LGBM
* Feature coefficient of LR


**Output and Conclusion:**
* Exited percentage is 20%
* LGBM performed best with AUC of 0.8507, precision 0.74 and recall 0.4
* LR's precision is around 0.6 but its recall outperformed the other two models
* I would focus more on accuracy and precision than recall since we do not want to take actions on "will exit customers" to keep them.
