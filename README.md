# Supply Chain Inventory Optimization: Pareto ABC Analysis

## Project Overview
Effective inventory management requires categorizing stock keeping units (SKUs) based on their economic impact. This project applies the **Pareto Principle (80/20 Rule)** to an industrial inventory portfolio, classifying items into strategic tiers (Class A, B, and C) based on Annual Usage Value to guide capital allocation, order policies, and supply chain control mechanisms.

## Methodology & Classification Rules
- **Annual Usage Value:** `Annual Demand (Units) × Unit Cost ($)`
- **Cumulative Percentage (%):** Running total of usage value divided by total portfolio inventory value ($212,210).
- **Classification Thresholds:**
  - **Class A (Strategic / High-Value):** Top ~75% of cumulative value (Strict control, continuous review, JIT replenishment).
  - **Class B (Moderate Importance):** Next ~20% of cumulative value (Periodic review, automated reorder points).
  - **Class C (Low-Value / High Bulk):** Bottom ~5% of cumulative value (Bulk purchasing, simplified safety stock policies).

## Portfolio Summary & Findings
| Category | SKU Count | % of Total Items | Total Annual Value ($) | % of Total Value | Inventory Strategy |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Class A** | 4 | 40.0% | $157,650 | 74.29% | Tight inventory monitoring, daily/weekly review, minimal safety stock |
| **Class B** | 3 | 30.0% | $41,750 | 19.67% | Standard control, monthly replenishment cycles |
| **Class C** | 3 | 30.0% | $12,810 | 6.04% | Bulk ordering, visual controls, high safety buffers |
| **Total** | **10** | **100.0%** | **$212,210** | **100.00%** | — |

## Visualization
The project features an automated **Pareto Combo Chart** in Excel combining clustered columns (descending individual usage values) with a secondary-axis cumulative percentage line, providing immediate operational insights for supply chain managers.

## Tools & Techniques
- **Microsoft Excel:** Dynamic array formulations (`SUMIF`, `COUNTIF`), descending sort automation, conditional nested `IF` statements, secondary-axis Pareto combo charting.
