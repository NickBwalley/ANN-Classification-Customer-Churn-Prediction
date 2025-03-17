# ANN-Classification-Customer-Churn-Prediction

This project uses an Artificial Neural Network (ANN) to predict customer churn based on input features such as Geography, Gender, Age, Balance, CreditScore, EstimatedSalary, Tenure, Number of Products, HasCreditCard, and IsActiveMember. The model classifies whether a customer is likely to churn or stay.

## Table of Contents

1. [Set-up Instructions](#set-up-instructions)
2. [Classification vs Regression](#classification-vs-regression)
3. [Understanding Dependent and Independent Features](#understanding-dependent-and-independent-features)

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

## Understanding Dependent and Independent Features

In machine learning, **dependent** and **independent** features play a crucial role in understanding data relationships and building predictive models. Below are clear explanations and relevant examples to help you understand each term.

## 1. Independent Features (Input Features)

**Definition:** These are the features (variables) that are used to predict an outcome. They are also known as **predictors**, **input variables**, or **explanatory variables**.

**Key Idea:** Independent features are what you feed into your model to make predictions.

### ✅ Example (Bank Churn Prediction Model)

Suppose you're building a model to predict if a customer will leave a bank (churn).

**Independent features (Inputs):**

- Age
- Credit Score
- Geography
- Balance
- Estimated Salary
- Tenure
- Number of Products
- Has Credit Card (Yes/No)
- Is Active Member (Yes/No)

These features influence the final prediction but are not the actual outcome.

---

## 2. Dependent Feature (Target/Output Feature)

**Definition:** This is the feature (variable) that you are trying to predict. It depends on the independent features.

**Key Idea:** The dependent feature is the outcome or result you want your model to predict.

### ✅ Example (Continuing the Bank Churn Example)

**Dependent feature (Target):**

- **Churn (Yes/No)** — The outcome that depends on the independent features.

---

## 3. Real-World Examples for Better Understanding

Here are a few relatable examples to help distinguish the two:

| **Scenario**                | **Independent Features (Inputs)**                     | **Dependent Feature (Target/Output)** |
| :-------------------------- | :---------------------------------------------------- | :------------------------------------ |
| House Price Prediction      | Number of rooms, Size of the house, Location          | House Price (in dollars)              |
| Student Exam Performance    | Study hours, Sleep quality, Class attendance          | Exam Score (percentage)               |
| Weather Forecasting         | Temperature, Humidity, Wind Speed                     | Chance of Rain (Yes/No)               |
| E-commerce Sales Prediction | Product category, Customer location, Discount offered | Number of Sales (units sold)          |

---

## 4. Key Difference in a Nutshell

- **Independent features** are the **cause** — the factors that influence the result.
- **Dependent feature** is the **effect** — the result you are trying to predict.

---

## 5. Quick Tip to Identify Them:

➡️ **Ask yourself:**

- "What am I trying to predict?" → **Dependent Feature**
- "What information do I have to make that prediction?" → **Independent Features**
