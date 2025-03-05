# 🚀 **Credit Risk Analysis**

## 📌 **Project Overview**

This project aims to **predict credit risk** using **Logistic Regression**, a machine learning classification model. The goal is to determine whether a loan is **healthy (0)** or **high-risk (1)** based on key financial indicators.

Understanding credit risk is crucial for financial institutions to make informed lending decisions, minimize defaults, and improve risk assessment models.

---

## 🔍 **Dataset & Features**

The dataset includes key financial metrics used to assess credit risk:

| **Feature Name**   | **Description**                             |
|--------------------|-------------------------------------------|
| `loan_size`       | The size of the loan                      |
| `interest_rate`   | The interest rate of the loan             |
| `borrower_income` | The borrower's annual income              |
| `debt_to_income`  | Ratio of total debt to total income       |
| `num_of_accounts` | Total number of accounts                  |
| `derogatory_marks`| Number of derogatory marks on credit      |
| `total_debt`      | Total outstanding debt                    |
| `loan_status`     | **Target variable** (0 = Healthy, 1 = High-Risk) |

---

## 🏗️ **Machine Learning Process**

### **1️⃣ Data Preprocessing**
- ✅ Cleaned missing values and ensured numerical consistency.
- ✅ Converted `loan_status` to an integer.
- ✅ Split data into **training (80%)** and **testing (20%)** sets.

### **2️⃣ Model Selection & Training**
- 📌 Implemented **Logistic Regression**, a widely used classification algorithm.
- 📌 Applied **class balancing** to improve model performance on minority classes.

### **3️⃣ Model Evaluation**
- 📊 Generated a **confusion matrix** and a **classification report**.
- 📊 Evaluated model performance using **accuracy, precision, recall, and F1-score**.

---

## 📈 **Results & Performance**

### **Logistic Regression Model Performance**
✅ **Accuracy:** **99%**  
✅ **Precision:**
   - **Healthy Loans (0):** 1.00
   - **High-Risk Loans (1):** 0.85
✅ **Recall:**
   - **Healthy Loans (0):** 0.99
   - **High-Risk Loans (1):** 0.99
✅ **F1-Score:**
   - **Healthy Loans (0):** 1.00
   - **High-Risk Loans (1):** 0.92

---

## 🔍 **Summary & Recommendations**

📌 The **logistic regression model performs exceptionally well** with **99% accuracy**. However:
- **Healthy loans (0) are predicted almost perfectly** (Precision: 1.00, Recall: 0.99).
- **High-risk loans (1) have slightly lower precision (0.85)**, meaning some healthy loans were misclassified as risky.

### 🔹 **Key Considerations**
- If the goal is to **reduce false positives** (avoid rejecting healthy loans incorrectly), improving **precision for high-risk loans** is necessary.
- If identifying **high-risk loans is critical**, the model is suitable as recall is very high (0.99).
- To improve performance, consider exploring **Random Forest** or **SVM models**.

### ✅ **Final Verdict**
💡 **This model is a strong candidate for credit risk prediction**, but fine-tuning may be required based on business priorities.

---

## 🛠️ **Installation & Usage**

To run this project on your local machine, follow these steps:

1. **Clone the repository:**
   ```bash
  [ git clone https://github.com/yourusername/credit-risk-analysis.git](https://github.com/Monse2604/credit-risk-classification.git)
   ```
2. **Navigate to the project directory:**
   ```bash
   cd credit-risk-analysis
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the analysis:**
   ```bash
   python credit_risk_analysis.py
   ```

---

## 📌 **Contributors**

- **Your Name** – [https://github.com/Monse2604]



