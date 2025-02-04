# Profit Maximization for Loan Sales

## Overview
This project aims to optimize the sale of two types of loans—cash loans and TV upgrade loans—to existing customers in 2023. The objective is to determine the best mix of these loans to maximize total profit while considering customer eligibility, loan constraints, and discount factors.

This project was developed as part of a data science hackathon and won first place.

## Problem Statement
We need to determine the best way to sell loans to our existing customers in 2023. Specifically, we have:
- **Cash Loans (Upsell Loans):** Extend the finished payment date of the original loan by 50 days and last for 150 days.
- **TV Upgrade Loans (Upgrade Loans):** Must be purchased the day the original loan is finished and cannot be upsold.

The goal is to maximize the total profit by optimizing the mix of these loans while considering eligibility rules, constraints, and financial discounting.

## Assumptions
- **Eligibility:**
  - 90% of customers are eligible for cash loans.
  - 75% of customers who haven’t purchased any upsell loans are eligible for a TV upgrade.
  - If a customer has already taken a cash loan, their eligibility for a TV upgrade decreases.
- **Loan Constraints:**
  - Cash loans cannot be taken after the original loan has finished payment.
  - TV upgrades must be purchased on the day the original loan is finished.
  - TV upgrades cannot be upsold.
- **Profit Calculation:**
  - Cash loans yield a profit of $150 on the day of sale.
  - A 15% annual discount rate is applied.
- **Time Scope:**
  - Only 2023 is considered; post-2023 impact is ignored.

## Approach
1. **Mathematical Formulation:**
   - Define an objective function to maximize total profit.
   - Establish constraints based on loan eligibility and timing.
2. **Optimization Techniques:**
   - Use Linear Programming (LP) or Dynamic Programming (DP) to determine the optimal mix of loans.
3. **Profit Calculation:**
   - Compute total profit based on the optimal allocation.
4. **Sensitivity Analysis:**
   - Evaluate critical assumptions and propose improvements for better profitability.

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/Abugahh/profit-max.git
   ```
2. Install dependencies .
3. Open `data.ipynb` and run the cells to view the analysis and optimization results.



