# 📊 Telco Customer Churn Prediction: Analysis and Modeling

## 📝 Project Description
The **Churn Rate** is one of the most critical metrics for telecommunications companies. Acquiring a new customer costs significantly more than retaining an existing one.
This project analyzes the "Telco Customer Churn" dataset to identify customer behaviors that indicate a propensity to leave. The ultimate goal is to build a Machine Learning model capable of predicting which users are at risk, allowing the company to intervene with targeted retention strategies.

## 🚀 Project Pipeline
The notebook follows an end-to-end workflow:

**Data Analysis and Data Cleaning**: General analysis of the dataset, handling missing values (e.g., TotalCharges), and correcting data types.

**Exploratory Data Analysis (EDA)**: Visualizing correlations between demographic variables, subscribed services, and contract types concerning Churn.

**Feature Engineering**: Encoding categorical variables and scaling numerical data.

**Model Building**: Implementing the Random Forest algorithm for prediction. 

**Evaluation**: Assessment based on business metrics such as Accuracy, Precision, Recall, F1-Score, and AUC.

## 📈 Key Insights (Analysis Examples)
During the exploratory analysis, several key points emerged:

**Month-to-month Contracts**: Customers with monthly contracts have a significantly higher churn rate.

**Payment Method**: Users paying via "Electronic check" tend to churn more frequently.

**Tenure**: The first 6 months are critical; if a customer surpasses their first year, the probability of churn drops drastically.

## 📊 Model Results
The final model achieved the following performance on the test set:
| Metric | Value | Notes |
| :--- | :--- | :--- |
| **Accuracy** | 0.7957 | Overall ability to predict the correct class. |
| **Precision** | 0.6625 | Ability to avoid classifying non-churners as churners. |
| **Recall** | 0.4724 | Ability to identify all customers who will actually churn. |
| **F1-Score** | 0.5515 | Harmonic mean of Precision and Recall; balances the cost of false positives and false negatives. |
| **ROC-AUC** | 0.8341 | The model's ability to distinguish between classes. |

## 🏁 How to Run the Project
1. Download the dataset [Kaggle: Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data)

2. Clone the repository:
```bash
git clone https://github.com/theofloris/Telco-Customer-Churn-Prediction.git
```
3. Navigate into the folder:
```bash

cd Telco-Customer-Churn-Prediction

```
4. Open the Notebook, load the dataset in the same folder (if using a local IDE). Upload it to the file section (if using Google Colab or Jupyter Notebook) and run the first cell.
