# **📌 Credit Risk Analysis Report**

🔍 Overview

This project analyzes credit risk using Logistic Regression, a machine learning model that predicts whether a loan is healthy (0) or high-risk (1). The dataset contains financial variables such as:

- Loan size

- Interest rate

- Borrower income

- Debt-to-income ratio

- Number of accounts

- Derogatory marks

- Total debt

The objective is to evaluate the model’s performance in classifying credit risk effectively.

📊 Dataset & Features

Feature Name

Description

loan_size

The size of the loan

interest_rate

The interest rate of the loan

borrower_income

The borrower's annual income

debt_to_income

Ratio of total debt to total income

num_of_accounts

Total number of accounts

derogatory_marks

Number of derogatory marks on credit

total_debt

Total outstanding debt

loan_status

Target variable (0 = Healthy, 1 = High-Risk)

🏗️ Machine Learning Process

1️⃣ Data Preprocessing

Cleaned missing values and ensured numerical consistency.

Converted loan_status to an integer.

Split data into training (80%) and testing (20%) sets.

2️⃣ Model Selection

Used Logistic Regression, a common classification algorithm.

Applied class balancing to handle the imbalance in high-risk loans.

3️⃣ Model Evaluation

Generated a confusion matrix and a classification report.

Evaluated model performance using accuracy, precision, recall, and F1-score.

📈 Results

Logistic Regression Model Performance

✅ Accuracy: 99%✅ Precision:

Healthy Loans (0): 1.00

High-Risk Loans (1): 0.85
✅ Recall:

Healthy Loans (0): 0.99

High-Risk Loans (1): 0.99
✅ F1-Score:

Healthy Loans (0): 1.00

High-Risk Loans (1): 0.92

🔍 Summary & Recommendations

📌 The logistic regression model performs exceptionally well with 99% accuracy. However:

Healthy loans (0) are predicted almost perfectly (Precision: 1.00, Recall: 0.99).

High-risk loans (1) have slightly lower precision (0.85), meaning some healthy loans were misclassified as risky.

🔹 Key Considerations

If the goal is to reduce false positives (avoid rejecting healthy loans incorrectly), improving precision for high-risk loans is necessary.

If identifying high-risk loans is critical, the model is suitable as recall is very high (0.99).

To improve performance, consider exploring Random Forest or SVM models.

✅ Final Verdict

💡 This model is a strong candidate for credit risk prediction, but fine-tuning may be required based on business priorities.
