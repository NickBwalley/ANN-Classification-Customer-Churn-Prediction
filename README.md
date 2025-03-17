# ANN-Classification-Customer-Churn-Prediction

This project uses an Artificial Neural Network (ANN) to predict customer churn based on input features such as Geography, Gender, Age, Balance, CreditScore, EstimatedSalary, Tenure, Number of Products, HasCreditCard, and IsActiveMember. The model classifies whether a customer is likely to churn or stay.

## Table of Contents

1. [Set-up Instructions](#set-up-instructions)
2. [Classification vs Regression](#classification-vs-regression)

---

## Set-up Instructions

1. **Create a new `venv`**

```bash
conda create -p venv python==3.11 -y
```

2. **Create your `requirements.txt` and install dependencies**

```bash
pip install -r requirements.txt
```

3. **Install `ipykernel` to run on `Jupyter Notebook`**

```bash
pip install ipykernel
```

---

## Classification vs Regression

Both **classification** and **regression** are types of supervised learning techniques used to predict outcomes, but they differ in the type of data they handle and the nature of their predictions. Let's break this down with real-world examples.

### 1. Classification

- **Definition:** Predicts **categories** or **classes** (discrete outcomes).
- **Output Type:** A **label** or **class** (e.g., Yes/No, Spam/Not Spam, etc.).

**Example Use Case:**  
Imagine you manage a **bank** and want to predict whether a customer will **default on a loan** or not.

- **Input Features:** Age, Income, Credit Score, Employment Status, etc.
- **Output (Prediction):**
  - **"Yes"** (Likely to default)
  - **"No"** (Unlikely to default)

Since the outcome has distinct categories, this is a **classification problem**.

### 2. Regression

- **Definition:** Predicts **continuous values** (numerical outcomes).
- **Output Type:** A **real number** (e.g., price, temperature, etc.).

**Example Use Case:**  
Suppose you are a **real estate agent** predicting the **price of a house**.

- **Input Features:** Number of rooms, Square footage, Location, Age of the house, etc.
- **Output (Prediction):**
  - **$250,000**, **$320,000**, **$450,000**, etc.

Since the outcome is a continuous number with no fixed categories, this is a **regression problem**.

### When to Use Each

- Use **classification** when predicting **categories** or **labels** (e.g., Spam/Not Spam, Fraud/Not Fraud, Cat/Dog).
- Use **regression** when predicting **continuous values** (e.g., Stock prices, Sales forecasts, Temperature predictions).

### Key Tip for Choosing the Right Model

- **Is the outcome a number that can take any value?** → **Regression**
- **Is the outcome one of a limited set of options?** → **Classification**

Both techniques are powerful, but choosing the right one depends on the type of data and the prediction goal.
