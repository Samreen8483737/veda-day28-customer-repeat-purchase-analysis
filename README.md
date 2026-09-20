# Day 28: Customer Repeat Purchase Analysis

## Objective
Measure repeat purchase behavior and segment customers to understand brand loyalty and long-term revenue metrics.

## Technical Implementation
* **Tools Used:** Python (Pandas, NumPy) and SQL (`sqlite3`).
* **Methodology:** 
  * Aggregated transactional data using Common Table Expressions (CTEs) to count distinct orders per `CustomerID`.
  * Classified customers logically: `OrderCount = 1` (First-Time) vs. `OrderCount > 1` (Repeat).
  * Calculated the overall Repeat Rate (percentage of total customer base with multiple purchases).
  * Executed a relational `JOIN` to compare the Average Order Value (AOV) between the two customer cohorts.

## Key Insights
1. **Strong Retention:** The business exhibits exceptional brand loyalty, with 77.22% of the customer base classified as repeat buyers. 
2. **AOV Discrepancy:** First-time buyers recorded a slightly higher Average Order Value ($281.23) compared to repeat buyers ($260.99). This suggests repeat customers might be making smaller, more frequent routine purchases, whereas new customers may be placing larger initial "bulk" orders.
