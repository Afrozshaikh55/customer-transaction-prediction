Customer Transaction Prediction
Project Overview
This project uses machine learning to predict whether a customer will make a transaction based on customer-related features.
The project covers data exploration, data quality checks, feature scaling, machine learning model comparison, and final model evaluation.
Dataset
The original dataset used for this project contains:
Rows: 200,000
Columns: 202
Target variable: target
The full original dataset is not included in this GitHub repository because of its large file size.
For this GitHub repository, a stratified sample of 10,000 rows from the original dataset is provided as:
data/train_sample.csv
The sample preserves the original target-class distribution and is intended to make the project lightweight and reproducible on GitHub.
Problem Statement
The goal is to build a classification model that predicts whether a customer will make a transaction:
1 → Customer makes a transaction
0 → Customer does not make a transaction
Project Workflow
Load the dataset
Perform initial data exploration
Check for missing values
Perform exploratory data analysis
Separate features and target
Split the data into training and testing sets
Scale the features using StandardScaler
Train multiple machine learning models
Compare models using ROC-AUC
Evaluate the selected model using classification metrics
Machine Learning Models
The following classification algorithms are compared:
Logistic Regression
Random Forest Classifier
K-Nearest Neighbors
Models are compared using cross-validation with ROC-AUC as the evaluation metric.
Evaluation Metrics
The final model is evaluated using:
Accuracy
Precision
Recall
ROC-AUC
Classification Report
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook
Project Structure
customer-transaction-prediction/
│
├── data/
│   └── train_sample.csv
│
├── notebooks/
│   └── customer_transaction_prediction.ipynb
│
├── .gitignore
├── README.md
└── requirements.txt
Notebook
The main project notebook is located at:
notebooks/customer_transaction_prediction.ipynb
The notebook loads the GitHub dataset using:
data = pd.read_csv("../data/train.csv")
How to Run
Clone the repository:
git clone <repository-url>
cd customer-transaction-prediction
Install the required libraries:
pip install -r requirements.txt
Open the notebook using Jupyter Notebook or JupyterLab and run the cells in order.
Author
Shaik Afroz
