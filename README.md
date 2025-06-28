# 📊 Supplier Risk Assessment using Machine Learning

> **Role:** Data Scientist  
> **Client:** Confidential (Global Supply Chain Client)  
> **Published:** Dec, 2024

---

## 🧾 Project Overview

Managing suppliers at scale is never easy — especially when some quietly become liabilities. In this project, I worked with a global logistics client to build a system that could automatically assess and flag suppliers based on risk. 

We trained a classification model to categorize suppliers as **High Risk**, **Medium Risk**, or **Low Risk**, based on how they performed across communication, delivery, and operational behavior. The idea was to give sourcing and procurement teams an early warning system — something data-backed that could complement their experience and instinct.

---

## 🧩 What We Looked At

To make this work, we combined data from a few key systems:

- 📬 **Communication logs** – e.g., how long it took suppliers to respond, how often conversations escalated  
- 📦 **Orders and requisitions** – cancellation rates, delivery timelines, fulfillment success  
- 🧾 **Supplier master records** – profile information, past compliance flags, regional context  

We had to clean and unify these datasets before doing any modeling — a lot of value came from just surfacing inconsistencies.

---

## 🎯 What We Wanted to Achieve

- Identify suppliers that could potentially become delivery risks  
- Give sourcing managers actionable insights to follow up on  
- Move beyond gut-feeling by showing clear, explainable risk scores  
- Help prioritize new onboarding reviews and contract renewals  

---

## 🧠 How We Approached It

We treated this as a supervised classification problem. Here’s the breakdown:

1. **Feature Engineering**  
   - Built features like `response_time_avg`, `order_delay_rate`, `escalation_ratio`, and `compliance_flag_count`  
   - Normalized supplier performance across regions and categories  

2. **Modeling & Evaluation**  
   - Tried several models (Random Forest, XGBoost) — XGBoost gave the best balance of precision and recall  
   - Used manually labeled data from past high-risk incidents as training targets  
   - Focused on interpretability using **SHAP** to explain why a supplier was tagged risky  

3. **Explainability First**  
   - Created per-supplier breakdowns showing which features contributed most to their risk label  
   - Shared results with stakeholders to validate that the model matched real-world intuition  

---

## 🛠 Tools & Techniques Used

| Area              | Stack                          |
|-------------------|-------------------------------|
| Language          | Python                         |
| Modeling          | Scikit-learn, XGBoost, SHAP    |
| Data Wrangling    | Pandas, NumPy                  |
| Collaboration     | Jupyter, Notion, Excel         |

---

## 📈 What It Delivered

- ⚠️ Surfaced risky suppliers that weren’t on the team's radar  
- 🔍 Provided clear, interpretable reasons for each classification  
- ⏱ Saved time by automating what was previously a manual review  
- ✅ Helped prioritize supplier audits and renewal decisions  

---

> ⚠️ **Note**: This repository does not contain code or data due to confidentiality. It serves as a case study to demonstrate problem-solving, data engineering, and machine learning skills in real-world projects.
