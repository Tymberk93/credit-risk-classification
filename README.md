# credit-risk-classification
## Module 20 - Credit Risk Assessment
### Analysis: </br>
* The purpose of this analysis is to build a model that can identify the creditworthiness of borrowers.</br>
* Dependant variable (y value) in this analysis was the "loan status" indicating if a loan is healthy or at risk. Independent Variables (x values) were loan size, interest rate, borrower income, debt to income ratio, number of accounts and derogatory marks.</br>
* In this analysis, we first split our data to traning and test sets. Then, define our dependent and independent variables. Next, we create logistic regression model and fit our original data to this model. Trained model is used to make predictions. Lastly, we evaluate the model`s performance.</br>
* Two diffeent Logistic Regression models were created by using the original data set and randomy over resampled data set (to get rid of the imbalances). In the end, their results -which was gathered with scikit-learn library- were compared.</br>

### Summary: </br>
<b> Logistic Regression Model with Origial Data </b></br>
![image](https://github.com/Tymberk93/credit-risk-classification/assets/120298970/dc3a2d85-a6c9-4b2b-a2dd-226af2f2dfee)</br>
![image](https://github.com/Tymberk93/credit-risk-classification/assets/120298970/60e2ad8f-57e7-492e-a3fd-bd3e2691fdf9)</br>

<b> Logistic Regression Model with Oversampled Data </b></br>
![image](https://github.com/Tymberk93/credit-risk-classification/assets/120298970/4525e3a8-e5e1-4460-b4f9-05d7cb31cd7a)
![image](https://github.com/Tymberk93/credit-risk-classification/assets/120298970/96327409-b7fd-43ee-8645-d46aae07d1e1)

<b> Analysis show that collected data can be effectively used to train and test the Machine Learning Classification Model. For better preditions solving the imbalance sampling issue is needed.

Randomly oversampling the data helps us to get higher balanced accuracy and recall scores. With higher recall value, model can predict risky loans more accurately.

With incorrect predictions we have two issues:

False positives (where users are flagged as risky, but are actually healthy)
False negatives (where users are not flagged as risky but are actually risky)
both cases have its costs. It is important to predict both 1s and 0s. Therefore, both models should have good accuracy.</b>
