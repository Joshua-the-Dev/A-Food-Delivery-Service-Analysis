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
- EXPECTED OUTCOMES

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
## Cost Analysis
### A breakdown of the associated costs is as follows:

| Cost Component             | Amount (INR)   |
|---------------------------|----------------|
| Refunds / Chargebacks     | ₹28,300.00      |
| Delivery Fees             | ₹28,620.00      |
| Payment Processing Fees   | ₹29,832.00      |
| Discount Fees             | ₹174,257.85     |
| **Total Costs**           | **₹261,009.85** |

## Profitability Evaluation
### The following key performance indicators (KPIs) were realized:

| Metric                      | Value        |
|----------------------------|--------------|
| Total Orders               | 1,000        |
| Total Revenue (Commission) | ₹126,990.00   |
| Total Costs                | ₹261,009.85   |
| **Net Profit**             | **₹-134,019.85** |

**Note:** This analysis reveals a negative net profit, indicating that costs exceed revenue. This suggests the food delivery service is currently operating at a loss, highlighting the need for cost optimization or revised pricing strategies to improve financial performance.

## Insights From the Analysis
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

<img width="642" alt="Screenshot 2025-05-06 134850" src="https://github.com/user-attachments/assets/9d7c1346-cbe8-48aa-8b60-d7d91e6b8434" />
<img width="644" alt="Screenshot 2025-05-06 140150" src="https://github.com/user-attachments/assets/b9f292d5-bc46-4e79-95d7-df2e3dc9ca30" />

# INSIGHTS
- Variable Commission Fees
  * Commission rates were inconsistent across orders, with an average commission of 19.75%.
  * This variability impacts revenue predictability and overall profitability.
- High Discount Costs
  * Total discount fees amounted to ₹174,257.85, accounting for 66.75% of total costs.
  * The 50% promotional offer alone made up 63.14% of these discount fees, significantly contributing to cost inflation.
- Unfavorable Cost-Revenue Ratio
  * Total costs were more than double the revenue earned through commissions, resulting in a negative profit margin.
- Order Trends by Day of the Week
  * Sundays recorded the lowest number of orders, indicating a natural downtime in operations.

# RECOMMENDATIONS
- Commission Structure
  * Renegotiate the commission rate to a minimum of 20% across all orders.
  * Ensure this rate is consistent and fixed, without exception, to maintain predictable revenue margins.
- Discount Policy
  * Temporarily suspend the 50% offer until further notice to reduce the financial burden caused by excessive discounts.
  * Evaluate the performance of future promotional campaigns more strategically.
  * Implement smarter, tiered promotional strategies to retain customers without incurring heavy losses.
- Payment Processing Optimization
  * Partner with trusted and cost-effective payment gateways that offer lower processing fees.
  * Prioritize reliability and fraud prevention when selecting payment processors.
- Delivery Route Optimization
  * Implement systems or tools to identify the fastest and most efficient delivery routes. For example Circuit for Teams, Onfleet, Google Maps, etc.
  * This will help reduce fuel consumption, delivery time, and overall delivery cost.
- Service Quality and Refund Reduction
  * Focus on improving service quality to minimize customer dissatisfaction.
  * Proactively work to reduce refunds and chargebacks through better order accuracy and support.
- Scheduled Maintenance
  * Perform scheduled maintenance, staff training, or system upgrades on Sundays, as it historically shows the lowest order volume.
  * This minimizes operational disruption and ensures the platform remains stable and efficient during peak days.

# Expected Outcomes
Implementing the recommended strategies will lead to:
- Increased and consistent revenue from a fixed 20% commission rate.
- Significant cost reduction by suspending the 50% discount and optimizing promotions.
- Lower payment processing and delivery costs through better tools and partners.
- Fewer refunds and chargebacks due to improved service quality.
- Minimal disruption from maintenance by scheduling it on low-demand Sundays.

**Overall, these changes are expected to transform the business from operating at a loss to achieving a positive profit margin of approximately 20.09% or higher.**
