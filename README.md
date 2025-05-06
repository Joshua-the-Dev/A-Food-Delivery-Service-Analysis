# OPTIMIZING COST AND PROFITABILITY: CASE STUDY FROM A FOOD DELIVERY SERVICE

# TABLE OF CONTENT
- FOOD ORDERS IN NEW DELHI - OVERVIEW
- OBJECTIVES OF THE ANALYSIS
- DATA SOURCE
- DESCRIPTION OF DATA
- TOOLS USED
- DATA PREPARATION
- DATA ANALYSIS
- DATA VISUALIZATION
- INSIGHTS
- RECOMMENDATIONS

# FOOD ORDERS IN NEW DELHI - OVERVIEW
This report analyzes the operational and financial performance of a food delivery service that is currently facing challenges in achieving profitability. Using a dataset of 1,000 food orders, the project aims to explore the key drivers of cost and revenue, evaluate the existing cost structure, and uncover insights into individual & overall profitability. The goal is to identify strategic opportunities for improving efficiency and profitability across the service's operations.

# OBJECTIVES OF THE ANALYSIS
The task was to conduct:
- Detailed Cost Analysis: Identify the major cost components associated with delivering food orders, including direct costs like delivery fees and indirect costs like discounts and payment processing fees.
- Profitability Evaluation: Calculate the profitability of individual orders and aggregate this data to assess overall profitability. This involves examining how revenue generated from commission fees measures against the total costs.
- Strategic Recommendations for Improvement: Based on the cost and profitability analysis, identify actionable strategies to reduce costs, adjust pricing, commission fees, and discount strategies to improve profitability. This includes finding a “sweet spot” for commission and discount percentages that ensures profitability across orders.
- Impact Simulation of Proposed Strategies: Simulate the financial impact of the recommended strategies on profitability, using the dataset to forecast how adjustments in commission rates and discount strategies could potentially transform current losses into profits.

# DATA SOURCE
The primary data is gotten from statso.io -[Download Here](https://statso.io/wp-content/uploads/2024/02/food_orders_new_delhi.csv)

# DESCRIPTION OF DATA
The original dataset contains the following columns:
- ORDER ID: A unique identifier assigned to each food order.
- CUSTOMER ID: A unique identifier for each customer who places an order.
- RESTAURANT ID: A unique identifier for each restaurant within the platform.
- ORDER DATA AND TIME: The date and time when the order was placed by the customer.
- DELIVERY DATE AND TIME: The date and time when the order was delivered to the customer.
- ORDER VALUE: The total monetary value of the order, including food, drinks, or any other items ordered.
- DELIVERY FEE: The amount charged to the customer for delivery services.
- PAYMENT METHOD: The method used by the customer to pay for the order.
- DISCOUNTS AND OFFERS: The promotional deals or percentage discounts applied to the order.
- COMMISSION FEE: The fee charged by the service or company for facilitating the order.
- PAYMENT PROCESSING FEE: The fee charged by the payment gateway for processing the transaction.
- REFUNDS/CHARGEBACKS: The amount refunded or reversed due to customer complaints, order issues, or disputes.

# TOOLS USED
- Microsoft Excel - Data analysis
- Microsoft Excel - Data visualization

# DATA PREPARATION
### Data Cleaning - The following data cleaning steps were performed using Power Query:
- Verified that there were no duplicate values in the dataset.
- Confirmed that no blank cells or missing values were present.
### Data Preprocessing - Several preprocessing steps were applied to standardize and structure the data:
- Numeric columns were formatted to display values with two decimal places for consistency.
- The "Discount and Offers" column was split into two separate columns "Discount" and "Offers" using the Text to Columns feature.
- In the "Discount" column, entries with "50" were standardized to "50%" and "none" was renamed to "0%".
- In the "Offers" column, "10%" was renamed to "Standard" and "0%" to "None".

<img width="960" alt="Screenshot 2025-05-06 121122" src="https://github.com/user-attachments/assets/f054c97e-5763-4588-9695-1bc501f736d8" />

# DATA ANALYSIS
## COST ANALYSIS
### A breakdown of the associated costs is as follows:

| Cost Component             | Amount (INR)   |
|---------------------------|----------------|
| Refunds / Chargebacks     | ₹28,300.00      |
| Delivery Fees             | ₹28,620.00      |
| Payment Processing Fees   | ₹29,832.00      |
| Discount Fees             | ₹174,257.85     |
| **Total Costs**           | **₹261,009.85** |

## PROFITABILITY EVALUATION
### The following key performance indicators (KPIs) were realized:

| Metric                      | Value        |
|----------------------------|--------------|
| Total Orders               | 1,000        |
| Total Revenue (Commission) | ₹126,990.00   |
| Total Costs                | ₹261,009.85   |
| **Net Profit**             | **₹-134,019.85** |

**Note:** This analysis reveals a negative net profit, indicating that costs exceed revenue. This suggests the food delivery service is currently operating at a loss, highlighting the need for cost optimization or revised pricing strategies to improve financial performance.

## INSIGHTS FROM THE ANALYSIS
- The average commission rate per order is approximately 19.75%, with variation observed across individual orders.
- Discount fees constitute about 66.75% of the total costs, indicating a major expense category.
- Orders with a 50% discount contribute roughly 63.14% of the total discount fees.
- The 10% standard discount offer was the most frequently applied, appearing in approximately 233 orders.

## Strategic Recommendations for Improvement
- Standardize and Increase Commission Rate:
The commission rate should be re-negotiated and increased by 0.25%, bringing it to a fixed 20% across all orders. This will help stabilize revenue and reduce variability in earnings per order.
- Suspend the 50% Off Promo Offer:
Given that the 50% discount contributes significantly (63.14%) to total discount fees but does not account for the majority of orders, it is advisable to temporarily suspend this offer. Doing so is expected to substantially lower overall discount related costs and improve net profit margins.

## Simulation of Proposed Strategies
- Revised Commission Calculation:
A new calculated column was created to apply a fixed 20% commission rate across all orders. This standardization allows for a clearer projection of revenue under the updated strategy. Additionally, orders with a 50% discount offer were excluded from the commission calculation to reflect their removal from the platform under the proposed strategy.
- Exclusion of 50% Off Promo Orders from Cost Calculations:
Using conditional logic (e.g., an IF statement), all orders with a 50% discount were excluded from the cost-related columns. New calculated columns were then generated to reflect the reduced discount fees, delivery fees, refunds/chargebacks and payment processing fees, simulating the financial impact of suspending the 50% off promo offer.

<img width="955" alt="Screenshot 2025-05-06 132404" src="https://github.com/user-attachments/assets/3e6d94c0-9819-456a-9aab-044d7828b18f" />

# DATA VISUALIZATION


