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

In this step the data was analyzed in terms of structure, features information, datatypes, missing data and statistics summary. Furthermore, features were selected and the data prepared to be used in the modeling.

**2.2 - Machine Learning Modeling**

For this project, seven ML models for classification: Naive Bayes (NB), Logistic Regression (LR), K-Nearest Neighbors (KNN), Suport Vector Machine (SVM), Random Forest (RF), Multilayer perceptron (MLP), Light Gradient Boosting Machine (LGBM) and XGBoost (XGB); were evaluted considering four metrics: Balanced Accuracy, Precision, Recall, F1 and Kappa; in a 5-fold cross validation strategy. Scalled and not scalled data were tested and hyperparameter tunning was done for the best model.
  
**2.3 - Company Expansion Strategy**

With the best model selected, a one time modeling was done and the results used to calculate the prospects of the company strategy using the model. Then, the questions of "The Challenge" were answered.
  
**2.4 - Model Deploy**

The one time model was saved and deployed. A small dataset was used to test the API and the model.
  
**2.5 - Report Writing**

A report with all relevant information obtained during the project was written.
  
## **3 - Data Analysis Report**
![image](https://user-images.githubusercontent.com/44379044/147887249-347b10c8-cbf1-4b46-949f-236926011b98.png)
![image](https://user-images.githubusercontent.com/44379044/147887255-102e0ef7-6ac1-486d-a9d0-3c247610541b.png)
![download](https://user-images.githubusercontent.com/44379044/172036574-e6a88e00-2fdb-4a88-91ec-db6d578babe7.png)
![image](https://user-images.githubusercontent.com/44379044/147887256-5454a9fa-1b3b-4585-b467-7fccc6a78683.png)

## **4 - Machine Learning Modeling Results**

| Model | Balanced Accuracy	| Precision	| Recall	| F1	| Kappa |
|:---------:|:-----------------:|:-----------:|:-----------:|:-----------:|:--------------:|
|LR & |	0.513 +/- 0.014 |	0.933 +/- 0.133 |	0.025 +/- 0.028 |	0.047 +/- 0.052 |	0.047 +/- 0.052 |
|NB	| 0.693 +/- 0.012 |	0.078 +/- 0.01 |	0.4 +/- 0.023 | 0.131 +/- 0.015 |	0.126 +/- 0.015 |
|SVM &	| 0.536 +/- 0.011	| 1.0 +/- 0.0	| 0.071 +/- 0.023 |	0.132 +/- 0.039	| 0.132 +/- 0.039 |
|NB & |	0.698 +/- 0.011 |	0.082 +/- 0.01 |	0.411 +/- 0.021	| 0.137 +/- 0.015	| 0.132 +/- 0.015 |
|LGBM &	| 0.691 +/- 0.1 |	0.275 +/- 0.2 |	0.386 +/- 0.201 |	0.309 +/- 0.197 |	0.306 +/- 0.198 |
|LGBM |	0.696 +/- 0.12 |	0.308 +/- 0.211 |	0.395 +/- 0.239 |	0.332 +/- 0.221 |	0.33 +/- 0.222 |
|SVM	| 0.621 +/- 0.012	| 0.995 +/- 0.01 |	0.242 +/- 0.024 |	0.389 +/- 0.031 |	0.388 +/- 0.031 |
|MLP &	| 0.694 +/- 0.019 |	0.913 +/- 0.051	| 0.387 +/- 0.037	| 0.543 +/- 0.044	| 0.543 +/- 0.044 |
|LR |	0.847 +/- 0.021 |	0.485 +/- 0.019 |	0.696 +/- 0.042 |	0.57 +/- 0.01 |	0.569 +/- 0.01 |
|MLP	| 0.903 +/- 0.065 |	0.529 +/- 0.23 |	0.81 +/- 0.133 |	0.584 +/- 0.147 |	0.582 +/- 0.148 |
|KNN	| 0.834 +/- 0.013	| 0.864 +/- 0.028 |	0.668 +/- 0.027 |	0.753 +/- 0.023 |	0.753 +/- 0.023 |
|KNN & |	0.863 +/- 0.011	| 0.918 +/- 0.015	| 0.727 +/- 0.022	| 0.811 +/- 0.014	| 0.811 +/- 0.014 |
|XGB	| 0.853 +/- 0.018	| 0.976 +/- 0.014	| 0.706 +/- 0.036	| 0.818 +/- 0.025	| 0.818 +/- 0.025 |
|XGB &	| 0.853 +/- 0.018	| 0.976 +/- 0.014	| 0.706 +/- 0.036	| 0.818 +/- 0.025	| 0.818 +/- 0.025 |
|RF & |	0.865 +/- 0.015	| 0.955 +/- 0.023	| 0.731 +/- 0.029	|0.827 +/- 0.02	| 0.827 +/- 0.02 |
|**RF**	| **0.865 +/- 0.013** | **0.961 +/- 0.021** | **0.729 +/- 0.026** | **0.829 +/- 0.017**	| **0.828 +/- 0.017** |

![image](https://user-images.githubusercontent.com/44379044/147887264-bfa7d1e0-75c6-411d-b534-daccf181f41a.png)
## **5 - Company Expansion Strategy**

## **6 - Conclusions and Prospects**

