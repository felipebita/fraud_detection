# **Fraudulent Transaction Detection**

This is a data science portfolio case proposed in the site [Seja Um Data Scientist](https://sejaumdatascientist.com/crie-uma-solucao-para-fraudes-em-transacoes-financeiras-usando-machine-learning/), the data set used is [Synthetic Financial Datasets For Fraud Detection](https://www.kaggle.com/ealaxi/paysim1).

## **1 - Business Understanding**
### 1.1 - Blocker Fraud Company
The Blocker Fraud Company is specialized in detecting fraudulent transactions made through mobile devices, the service Blocker Fraud ensures the blocking of those transactions. The company's business model is of the Service type, with monetization made by the performance of the service provided, that is, the user pays a fixed fee on the success in detecting fraud in the client's transactions.
### 1.2 - Expansion Strategy
A very agressive strategy:
*   The company will receive 25% of the value of each transaction that is truly detected as fraud.
*   The company will receive 5% of the value of each transaction detected as fraud, however the transaction is truly legitimate.
*   The company will return 100% of the value to the customer for each transaction detected as legitimate, however the transaction is truly a fraud.

### 1.3 The Challenge
You have been hired as a Data Science Consultant to create a highly accurate fraud detection model. You need to provide a model in production where clients will send their transactions via API to be classified as fraudulent or legitimate. In addition, you need to submit a report containing your model's performance and the profit that the company will make using the service. Your report should contain the answers to the following questions:
*   What is the model's Precision and Accuracy?
*   How Reliable is the model in classifying transactions as legitimate or fraudulent?
*   What is the Expected Billing by the Company if we classify 100% of transactions with the model?
*   What is the Loss Expected by the Company in case of model failure?
*   What is the Profit Expected by the Blocker Fraud Company when using the model?
