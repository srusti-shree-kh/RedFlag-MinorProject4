# 🚩 RedFlag – The Fraud Files

### SQL-Based Financial Transaction Fraud Detection

## 📌 Project Overview

RedFlag – The Fraud Files is a SQL-based fraud detection project designed to identify suspicious financial transaction patterns in a fictional Indian payment aggregator called **PayFast**.

The project uses MySQL to analyze approximately 200,000 synthetic transactions and investigate 12 potentially suspicious transaction patterns. It demonstrates the practical application of SQL in financial data analysis and fraud detection.

## 🎯 Project Objectives

- Identify suspicious transaction patterns using SQL.
- Analyze transaction frequency, amounts, status, and timestamps.
- Detect unusual user and merchant behavior.
- Apply SQL concepts to a financial fraud detection scenario.
- Develop practical skills in SQL and data analytics.

## 🛠️ Technologies Used

- **Database:** MySQL
- **Query Language:** SQL
- **Database Tool:** MySQL Workbench
- **Domain:** Data Analytics
- **Business Domain:** Financial Fraud Detection and FinTech Analytics

## 📊 Dataset Information

The project uses synthetic transaction data from a fictional payment aggregator named PayFast.

- **Dataset Size:** Approximately 200,000 transactions
- **Analysis Period:** January 1 – June 30, 2024
- **Database Table:** `transactions`
- **Number of Columns:** 9
- **Data Type:** Synthetic financial transaction data

### Dataset Columns

| Column Name | Description |
|---|---|
| `txn_id` | Unique transaction identifier |
| `user_id` | Identifier of the user initiating the transaction |
| `merchant_id` | Identifier of the merchant involved |
| `amount` | Transaction amount |
| `txn_time` | Date and time of the transaction |
| `status` | Transaction status |
| `payment_mode` | Payment method used |
| `city` | City associated with the transaction |
| `txn_type` | Type of transaction |

## 🔍 Fraud Detection Patterns

The project investigates 12 potentially suspicious transaction patterns using SQL.

### 1. Velocity Fraud
Identifies users making an unusually high number of transactions within a single day.

### 2. Round-Amount Clustering
Detects repeated round-number transaction amounts that may indicate suspicious activity.

### 3. Card Testing
Identifies repeated low-value transactions that may indicate attempts to test payment card validity.

### 4. Failed-Then-Succeeded Transactions
Examines cases where failed transactions are followed by successful transactions.

### 5. Odd-Hour Concentration
Analyzes transaction activity during unusual hours to identify potentially suspicious behavior.

### 6. Mule Accounts
Investigates rapid movement of funds through accounts that may be used to transfer suspicious money.

### 7. Refund Abuse
Identifies unusual refund patterns that may indicate possible misuse of the refund process.

### 8. Merchant Collusion
Examines potentially suspicious transaction relationships involving merchants.

### 9. Structuring Around the KYC Threshold
Identifies transactions clustered just below the ₹10,000 threshold that may require further investigation.

### 10. Dormant-Then-Active Accounts
Detects previously inactive accounts that suddenly begin showing transaction activity.

### 11. Velocity Spike
Identifies unusual increases in transaction activity compared with typical activity.

### 12. Geographic Impossibility
Identifies transactions associated with the same user in different cities within a short time interval using SQL time-based analysis.

*These queries flag potentially suspicious activity for further investigation; they do not independently prove that fraud has occurred.*

## 🧠 SQL Concepts Demonstrated

- `SELECT`, `WHERE`, and `ORDER BY`
- Aggregate functions such as `COUNT()`, `SUM()`, and `AVG()`
- `GROUP BY` and `HAVING`
- Joins and subqueries
- Common Table Expressions (CTEs)
- Window functions such as `LAG()`
- Conditional logic
- Date and time analysis
- `TIMESTAMPDIFF()`
- Transaction aggregation and pattern analysis

## 📁 Repository Structure

```text
RedFlag-MinorProject4/
│
├── README.md
└── redflag.sql
```

### File Description

- **README.md:** Contains the project overview, objectives, technologies, dataset information, fraud detection patterns, and execution instructions.
- **redflag.sql:** Contains the 12 final SQL fraud detection queries with comments and findings.

**Dataset Note:** The large `redflag_transactions.sql` dataset file is kept separate from this GitHub repository. It can be shared through Google Drive if required.

## ▶️ How to Run the Project

### Prerequisites

- MySQL Server
- MySQL Workbench
- The project dataset SQL file

### Execution Steps

1. Install and open MySQL Workbench.
2. Connect to your MySQL Server.
3. Obtain the `redflag_transactions.sql` dataset file separately.
4. Review and execute the dataset setup script to create and populate the `redflag` database.
5. Verify that the `transactions` table has been created and populated.
6. Download or open `redflag.sql` from this repository.
7. Execute the fraud detection queries individually or in sections.
8. Review the results to investigate potentially suspicious transaction patterns.

**Important:** Review the dataset setup script before running it. It may contain a `DROP DATABASE IF EXISTS redflag` statement, which can delete an existing database named `redflag`.

## 📈 Project Outcomes

- Developed 12 SQL queries to investigate potentially suspicious financial transaction patterns.
- Applied SQL to analyze transaction behavior and identify unusual activities.
- Practiced aggregation, joins, subqueries, CTEs, and window functions.
- Explored transaction velocity, refund activity, merchant behavior, and geographic anomalies.
- Gained practical experience relevant to SQL, data analytics, and fraud analytics roles.

## 👩‍💻 Author

**Srusti Shree K H**

## 📑 Project Information

- **Project Name:** RedFlag – The Fraud Files
- **Project Type:** Minor Project
- **Domain:** Data Analytics
- **Business Domain:** Financial Fraud Detection and FinTech Analytics
- **Database:** MySQL
- **Core Technology:** SQL
- **Dataset Size:** Approximately 200,000 synthetic transactions
- **Analysis Period:** January–June 2024
- **Dataset:** Fictional PayFast transaction data
- **Fraud Detection Patterns:** 12
- **Purpose:** Academic learning and practical application of SQL-based fraud detection.

---

*This project was developed for educational purposes using a fictional payment aggregator and synthetic transaction data. It demonstrates the application of SQL for identifying suspicious transaction patterns, analyzing unusual financial activities, and supporting financial fraud investigations.*
