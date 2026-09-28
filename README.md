# 💳 Credit Risk & Loan Portfolio Analytics Dashboard

An end-to-end data analytics project examining borrower risk factors, default predictors, and loan portfolio health using **Excel** and **Power BI**. 

---

## 📌 Project Overview
Lending institutions face constant exposure to financial defaults. This project analyzes a comprehensive historical loan dataset to identify the core drivers of loan defaults (`loan status`), evaluate portfolio risk exposure, and segment borrowers by creditworthiness and debt-to-income thresholds.

The goal of this dashboard is to answer critical risk questions: *Who is most likely to default? At what debt threshold do borrowers fail? And how effectively do credit scores predict default behavior?*

---

## 📊 Dataset & Features
The dataset contains **14 key borrower and loan attributes**:
* **Demographics & Profile:** `person age`, `person gender`, `person education`, `person income`, `person emp exp` (employment experience), `person home ownership`.
* **Loan Details:** `loan amount`, `loan intent` (personal, education, venture, medical, home improvement, debt consolidation), `loan interest rate`, `loan percent income`.
* **Credit History & Risk:** `credit score`, `cb person cred hist length`, `previous loan defaults on file` (Yes/No), `loan status` (0 = Repaid/Active, 1 = Defaulted).

---

## 🔍 Key Business Questions Addressed
1. **Portfolio Default Rate:** What is the overall default rate across the historical portfolio, and how much capital is locked in defaulted loans?
2. **The Debt Cliff:** At what percentage does `loan percent income` trigger a massive spike in defaults?
3. **Credit Score Impact:** How reliably do credit score status (*Poor, Fair, Good, Excellent*) separate high-risk borrowers from safe ones?
4. **Behavioral Risk:** How heavily does having a `previous loan defaults on file` increase current default probability?
5. **Intent Analysis:** Which `loan intent` categories carry the highest default risk relative to their total volume?

---

## 🛠️ Tools & Workflow
* **Data Cleaning & Preparation (Excel):** Checked for missing values, standardized categories, and created custom calculated risk tiers.
* **Visualization & Reporting (Power BI):** Designed a 2-page interactive executive dashboard featuring custom DAX measures for default rates, capital at risk, and risk segmentation.

---

## 📈 Power BI Dashboard Preview

> *<img width="1920" height="1080" alt="Screenshot (78)" src="https://github.com/user-attachments/assets/3b292e40-27f0-4c6a-a2f3-089ba594f34d" />
*
*Page 1: Portfolio Overview, Default Rates by Loan Intent, and Home Ownership Split.*

> *<img width="1920" height="1080" alt="Screenshot 2026-09-28 110720" src="https://github.com/user-attachments/assets/734e8cec-0c9d-4f6c-9fe2-d4cf82028684" />
*
*Page 2: Credit Score Impact, Income vs. Loan Amount Risk Tiers, and Previous Defaults Analysis.*

---

## 💡 Key Insights & Strategic Recommendations
* **The Debt-to-Income Tipping Point:** Defaults surge dramatically once a loan exceeds **40%** of a borrower's annual income, suggesting stricter caps should be placed on high debt-to-income ratio approvals.
* **Credit Score Reliability:** While poor credit scores (<580) exhibit high default rates, mid-tier brackets require closer scrutiny regarding employment stability (`person emp exp`) before approval.
* **Past Behavior Predicts Future Risk:** Borrowers with previous defaults on file show a exponentially higher repeat-default rate, indicating that past history should carry heavier weight in automated underwriting rules.

---

## 🚀 How to View This Project
1. Clone or download this repository.
2. Open the `.pbix` file in **Power BI Desktop** to interact with the dashboard.
3. Review the cleaned dataset in the `data/` folder.
