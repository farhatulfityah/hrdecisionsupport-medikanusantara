# HR Decision Support System — Medika Nusantara

This project is a prototype of an AI-powered HR decision support system designed to help HR managers make better workforce decisions, particularly around employee attrition and internal mobility.

The system demonstrates how **data quality directly impacts decision-making**, not just model output.

---

## 🎯 Problem Statement

In real enterprise environments, HR data is often:
- Incomplete (missing skills, performance history)
- Inconsistent (different job titles for the same role)
- Fragmented across systems (HRIS, ATS, LMS)

As a result:
- AI predictions become unreliable
- Decisions may be incorrect or require manual validation

This project focuses on solving that problem through a **data layer + decision interface**, not just predictive modeling.

---

## 💡 Solution Overview

The system provides a decision interface for HR managers with:

- **Attrition Risk (%)** — probability of employee leaving in the next 6 months  
- **Confidence Score** — reliability of prediction based on data quality  
- **Action Recommendation** — clear next step (e.g., retention, review, internal move)  

The goal is to enable **actionable decisions without requiring users to understand the AI model**.

---

## 🧪 Synthetic Data (Deliverable 3)

Two datasets are generated to simulate real-world conditions:

### Dataset A — Messy (Enterprise Reality)
- ~200 employees
- Missing skills (~40%)
- Inconsistent job titles
- Incomplete performance records
- Conflicting or duplicate-like entries

### Dataset B — Clean (Post-Processing)
- Standardized job titles
- Missing values inferred where possible
- Records normalized and consolidated
- Confidence score assigned to each employee
- Low-confidence records flagged for human review

---

## 🔍 Key Insight

> The same employee can produce different decisions depending on data quality.

- In **messy data**, confidence is low → more "Review Required"
- In **clean data**, confidence improves → more actionable decisions

This highlights that:
> **The value of AI systems depends heavily on the quality of the data layer, not just the model.**

---

## 🖥️ Features

- Toggle between **Clean Data** and **Messy Data**
- Employee-level decision view
- Confidence-based decision logic
- Warning system for low-quality data
- CSV export for both datasets
- Realistic multi-department workforce (Clinical, HR, Sales, Engineering, etc.)

---

## ⚙️ How to Run

1. Download or clone this repository
2. Open `index.html` in your browser
3. No installation required

---

## 🧠 Design Principles

- **Decision-first, not model-first**
- **Transparency over false certainty**
- **Actionability over analytics complexity**
- **Trust through clarity and consistency**

---

## 🚀 Future Improvements

- Highlight cases where decisions change between messy and clean data
- Add data quality dashboard (missing, inferred, conflicting fields)
- Improve role-specific decision logic (e.g., clinical vs corporate roles)

---
