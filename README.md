# Customer Intelligence Agent

This project showcases an AI-powered agent designed to transform raw Excel data into actionable business insights using natural language queries. Built on the ReAct framework (Reasoning + Acting), the agent goes beyond simple SQL translation to perform dynamic reasoning, predictive simulations, and business-level interpretation.

## 🔍 Problem Statement

Marketing teams often struggle with:
- Manually filtering and calculating derived metrics (e.g., days since last transaction)
- Defining fuzzy business terms like "high-value" or "inactive"
- Combining multiple conditions (location + spend + inactivity)
- Scaling queries across large datasets

## 💡 Solution

This agent solves all of the above with a single natural language query like:
> “Find high-value inactive customers in Mumbai.”

It understands business rules, applies logic, and returns:
- A list of matching customers
- A summary insight (e.g., “10 inactive premium customers in Mumbai, avg spend ₹45k”)
- Suggested actions (e.g., re-engagement campaign)

## 🧠 Key Features

- **ReAct Framework**: Reason → Act → Iterate
- **Business Rule Engine**: Interprets fuzzy terms like churn risk, loyalty, inactivity
- **Tool Integration**:
  - SQLDatabaseToolkit
  - Simulation tools: churn, affinity, lifetime value
- **Data Enrichment**:
  - Added columns: demographics, referrals, subscriptions, derived metrics
- **Clustering & PCA**:
  - KMeans for customer segmentation
  - PCA for dimensionality reduction

## 📊 Dataset Enhancements

Original Excel was shallow. We enriched it with:
- **Demographics**: age, gender, occupation, location
- **Transactions**: last_transaction_date, total_transaction_amount, etc.
- **Engagement**: login_days, support_tickets
- **Referrals & Subscriptions**
- **Derived Metrics**: days_since_last_transaction, days_since_last_login

## 🧪 Predictive Capabilities

- **simulate_churn**: churn probability
- **simulate_affinity**: next likely product
- **simulate_ltv**: lifetime value

## 🚀 Why It Matters

Unlike traditional SQL analysts, this agent:
- Understands business language
- Applies hidden logic dynamically
- Handles synonyms and categories
- Presents results in plain summaries for non-technical users

## 📦 Tech Stack

- Python
- SQLite
- LangChain (ReAct agent)
- Pandas, Scikit-learn
- Custom simulation modules

---

