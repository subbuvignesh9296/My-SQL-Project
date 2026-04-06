**E-Commerce Customer Churn Analysis - MySQL Project**
**Project Overview**
This project focuses on analyzing customer churn for an e-commerce platform using MySQL. Churn analysis helps in identifying customers who are likely to stop using a service, allowing the business to take proactive measures for retention. The analysis covers various factors such as customer demographics, login behavior, payment modes, and satisfaction scores.

**Database Structure**
The project utilizes a database named ecomm with a primary table customer_churn.

**Table: customer_churn**
This table contains detailed information about each customer:

**CustomerID:** Unique identifier for the customer (Primary Key).

**Churn:** Binary indicator of whether the customer has churned (1) or not (0).

**Tenure:** How long the customer has been with the platform.

**PreferredLoginDevice:** The device usually used by the customer to login (e.g., Mobile Phone, Computer).

**CityTier:** Categorization of the customer's city.

**WarehouseToHome:** Distance from the warehouse to the customer's home.

**PreferredPaymentMode:** The customer's most used payment method (e.g., Debit Card, UPI, CC).

**Gender:** Male or Female.

**HourSpendOnApp:** Average hours spent on the application.

**NumberOfDeviceRegistered:** Total devices the customer has registered.

**PreferedOrderCat:** Favorite category of items ordered (e.g., Laptop & Accessory, Mobile, Fashion).

**SatisfactionScore:** Customer satisfaction rating.

**MaritalStatus:** Single, Married, or Divorced.

**NumberOfAddress:** Total addresses registered by the customer.

**Complain:** Whether the customer has raised a complaint (1 for Yes, 0 for No).

**OrderAmountHikeFromlastYear:** Percentage increase in order amount compared to the previous year.

**CouponUsed:** Number of coupons used in the last month.

**OrderCount:** Total number of orders placed in the last month.

**DaySinceLastOrder:** Number of days since the customer's last order.

**CashbackAmount:** Average cashback received in the last month.

**Key Analysis & Queries**
**The SQL script provides several analytical queries to understand churn patterns:**

**1. Retention & Behavior Analysis**
Gender-based Coupon Usage: Identifies which gender utilizes the highest number of coupons to target marketing efforts.

Login Device & Marital Status: Analyzes specific segments, such as single customers using mobile phones, to understand their behavior.

High-Value Customers: Identifies married customers in Tier-1 cities whose order count is above the average.

**2. Operational Insights**
Distance Breakdown: Categorizes the distance from WarehouseToHome (Very Close, Close, Moderate, Far) and calculates churn rates for each category.

Returns Tracking: A secondary table customer_returns is created to track ReturnID, CustomerID, ReturnDate, and RefundAmount to analyze return trends and their impact on satisfaction
