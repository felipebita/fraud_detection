![fraud](https://user-images.githubusercontent.com/44379044/131612132-7b78ceaa-09f9-4eef-b86a-b3979fae2909.png)

# **Fraudulent Transaction Detection**

This is a not finished data science project, the business problem is proposed by [Seja Um Data Scientist](https://sejaumdatascientist.com/crie-uma-solucao-para-fraudes-em-transacoes-financeiras-usando-machine-learning/), using the data set [Synthetic Financial Datasets For Fraud Detection](https://www.kaggle.com/ealaxi/paysim1).

## **1 - Business Understanding**
### 1.1 - Blocker Fraud Company
The Blocker Fraud Company is specialized in detecting fraudulent transactions made through mobile devices, the service Blocker Fraud ensures the blocking of those transactions. The company's business model is of the Service type, with monetization made by the performance of the service provided, that is, the user pays a fixed fee on the success in detecting fraud in the client's transactions.

### 1.2 - Expansion Strategy
A very agressive strategy:
*   The company will receive 25% of the value of each transaction that is truly detected as fraud.
*   The company will receive 5% of the value of each transaction detected as fraud, however the transaction is truly legitimate.
*   The company will return 100% of the value to the customer for each transaction detected as legitimate, however the transaction is truly a fraud.

### 1.3 - The Challenge
You have been hired as a Data Science Consultant to create a highly accurate fraud detection model. You need to provide a model in production where clients will send their transactions via API to be classified as fraudulent or legitimate. In addition, you need to submit a report containing your model's performance and the profit that the company will make using the service. Your report should contain the answers to the following questions:
*   What is the model's Precision and Accuracy?
*   How Reliable is the model in classifying transactions as legitimate or fraudulent?
*   What is the Expected Billing by the Company if we classify 100% of transactions with the model?
*   What is the Loss Expected by the Company in case of model failure?
*   What is the Profit Expected by the Blocker Fraud Company when using the model?

## **2 - Solution Strategy**
A data science project was developed to build, evaluate and launch a machine learning model capable of classifying transactions as fraudulent or legitimate. The project consists of the following steps:

**2.1 - Data Analysis and Preparation**

**2.2 - Machine Learning Modeling**

**2.3 - Company Expansion Strategy**

**2.4 - Model Deploy**

**2.5 - Report writing**

## **3 - Data Analysis Report**

## **4 - Machine Learning Modeling Results**
|Model| Balanced Accuracy |  Precision  |    Recall   |      F1     |      Kappa     |
|:---------:|:-----------------:|:-----------:|:-----------:|:-----------:|:--------------:|
|Dummy|   0.5 +/- 0.001 |	0.001 +/- 0.003 |	0.001 +/- 0.003 |	0.001 +/- 0.003	| 0.0 +/- 0.003 |
|Dummy &|0.501 +/- 0.002	|0.002 +/- 0.003|	0.002 +/- 0.003|	0.002 +/- 0.003|	0.001 +/- 0.003|
|NaiveBayes &|	0.785 +/- 0.004	|0.003 +/- 0.0|	0.991 +/- 0.009	|0.006 +/- 0.0	|0.004 +/- 0.0|
|Logistic Regression scld|	0.505 +/- 0.006|	0.567 +/- 0.467|	0.01 +/- 0.012|	0.02 +/- 0.022|	0.02 +/- 0.022|
|NaiveBayes|	0.576 +/- 0.01|	0.07 +/- 0.015|	0.154 +/- 0.02|	0.096 +/- 0.019|	0.094 +/- 0.019|
|SVM &|	0.533 +/- 0.006|	1.0 +/- 0.0|	0.066 +/- 0.012|	0.124 +/- 0.021|	0.124 +/- 0.021|
|LGBM &|	0.603 +/- 0.097|	0.169 +/- 0.127|	0.208 +/- 0.194|	0.183 +/- 0.153|	0.182 +/- 0.153|
|LGBM|	0.603 +/- 0.097|	0.169 +/- 0.127|	0.208 +/- 0.194|	0.183 +/- 0.153|	0.182 +/- 0.153|
|MLP|	0.803 +/- 0.092|	0.286 +/- 0.155|	0.615 +/- 0.178|	0.352 +/- 0.166|	0.351 +/- 0.166|
|SVM|	0.622 +/- 0.011|	0.995 +/- 0.009|	0.243 +/- 0.022|	0.39 +/- 0.028|	0.39 +/- 0.028|
|Logistic Regression|	0.844 +/- 0.073|	0.39 +/- 0.23| 0.689 +/- 0.146|	0.432 +/- 0.073|	0.431 +/- 0.073|
|MLP &|	0.673 +/- 0.012	|0.912 +/- 0.074|	0.346 +/- 0.024|	0.501 +/- 0.032|	0.5 +/- 0.032|
|KNeighborsClassifier|	0.804 +/- 0.015|	0.843 +/- 0.033|	0.608 +/- 0.03|	0.706 +/- 0.028	|0.705 +/- 0.028|
|XGB|	0.842 +/- 0.022	|0.975 +/- 0.014|	0.683 +/- 0.043|	0.803 +/- 0.029|	0.802 +/- 0.029|
|XGB &|	0.842 +/- 0.022|	0.975 +/- 0.014|	0.683 +/- 0.043|	0.803 +/- 0.029|	0.802 +/- 0.029|
|KNeighborsClassifier &|	0.866 +/- 0.015|	0.918 +/- 0.024|	0.732 +/- 0.03|	0.814 +/- 0.02|	0.813 +/- 0.02|
|Random Forest &|	0.87 +/- 0.018|	0.95 +/- 0.017|	0.741 +/- 0.036|	0.832 +/- 0.025|	0.832 +/- 0.025|
|**Random Forest**|**0.872 +/- 0.019**	|**0.958 +/- 0.013**|**0.744 +/- 0.037**	|**0.837 +/- 0.024**	|**0.837 +/- 0.024**|

## **5 - Company Expansion Strategy**

## **6 - Conclusions and Prospects**

