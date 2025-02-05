# Loan-Portfolio-Performance-Analysis

Loan Portfolio Performance Analysis

Overview
This SQL-based project analyzes a loan portfolio to track default rates, revenue trends, and customer risk segmentation using structured query language (SQL).

Technologies Used

MySQL for database management
SQL Functions Used:
COUNT(), SUM(), CASE WHEN, AVG()
GROUP BY, ORDER BY
DATE_TRUNC(), INTERVAL
Subqueries for customer segmentation
Key Features

Loan Default Rate Analysis: Determines the percentage of defaulted loans.
Revenue Trend Analysis: Forecasts monthly payments collected.
Customer Segmentation: Classifies customers into Low, Moderate, and High Payers based on repayment behavior.
Database Schema

loan_portfolio

loan_id (INT, PK) - Unique loan identifier
customer_id (INT) - Associated customer ID
loan_amount (DECIMAL(10,2)) - Loan principal amount
interest_rate (DECIMAL(5,2)) - Interest rate for the loan
term (INT) - Loan term in months
status (ENUM: Current, Defaulted, Paid-off) - Loan status
credit_score (INT) - Customer credit score
income (DECIMAL(10,2)) - Customer's annual income
employment_status (VARCHAR(50)) - Employment status
payments

payment_id (INT, PK) - Unique payment identifier
loan_id (INT, FK) - Associated loan ID
customer_id (INT, FK) - Associated customer ID
payment_date (DATE) - Date of payment transaction
amount_paid (DECIMAL(10,2)) - Payment amount made
