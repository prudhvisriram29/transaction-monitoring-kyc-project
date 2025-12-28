# KYC Transaction Monitoring Project (Rule-Based Analysis)

## 📌 Overview
This project simulates suspicious transaction monitoring using rule-based logic aligned with KYC/AML workflows.  
The goal is to identify potential high-risk transactions that may require enhanced due diligence or manual investigation.

## 🎯 Objectives
- Identify high-value transactions
- Detect rapid multiple transactions using time difference
- Classify transactions based on defined thresholds
- Generate summary metrics and a monitoring report

## 🧠 Rules Used
| Rule | Condition | Meaning |
|-------|----------|---------|
| High-value transaction | Amount > 1000 | Requires attention; potential EDD |
| Low-value transaction | Amount ≤ 1000 | Lower risk, unless frequent |
| Rapid multiple transactions | Time_Diff < 60 sec | Could indicate structuring or layering |

> Thresholds were calibrated to reflect dataset scale and simulate AML scenarios.

## 📊 Key Metrics from Summary Sheet
- Total transactions: **284,807**
- High-value transactions: **9,262**
- Low-value transactions: **275,665**
- Flagged transactions: **184,431**
- Not flagged: **100,376**

## 📂 Folder Structure
