# Hotel Booking Cancellation Predictor

A machine learning project that predicts the probability of a hotel booking being canceled, helping revenue‐management teams minimize losses and optimize capacity planning.

## 📋 Project Overview

- **Objective**  
  Predict whether a hotel reservation will be canceled (`is_canceled`) based on historical booking data.

- **Key Features**  
  - **Lead time**: days between booking and arrival  
  - **Stay length**: number of weekend vs. weekday nights  
  - **Group composition**: adults, children, babies  
  - **Meal plan**: BB, HB, FB, SC, etc.  
  - **Average daily rate (ADR)**  
  - **Customer history**: previous cancellations, repeat guest flag  
  - **Booking channel & deposit type**

## 🛠️ Workflow

1. **Data Cleaning**  
   - Remove contradictory records (e.g. confirmed booking with zero nights stayed)  
   - Fill or flag missing values appropriately  
   - Drop or simplify non‑essential columns  

2. **Feature Engineering**  
   - Compute total nights stayed  
   - Encode categorical variables (meal type, market segment, etc.)  
   - Derive new indicators (e.g. “has_special_requests”)  

3. **Modeling & Evaluation**  
   - Train classification algorithms (Logistic Regression, Random Forest, etc.)  
   - Evaluate with accuracy, precision, recall, F1‑score & ROC AUC  
   - Analyze feature importance to uncover drivers of cancellation  

## 🎯 Outcome

A lightweight, deployable model that flags high‑risk cancellations in real time and provides actionable insights to improve booking strategies and customer retention.

---

*Feel free to explore the Jupyter notebooks and scripts in this repo to follow each step of the process.*  
