# Retail Store Monthly Sales Regression Analysis

## Business Problem Summary

The leadership team of a retail chain wants to understand which business factors are most strongly associated with monthly sales performance across stores. The objective is to support decisions regarding marketing investment, inventory management, staffing, pricing strategy, and store operations using regression analysis.

---

# Dataset Description

The dataset contains monthly operational and financial performance for multiple retail stores.

Variables include:

- store_id
- month
- region
- store_type
- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- competitor_distance_km
- holiday_flag
- customer_rating
- monthly_sales
- monthly_profit

---

# Dependent Variable

- monthly_sales

---

# Independent Variables

Numerical Variables

- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- competitor_distance_km
- customer_rating
- holiday_flag

Categorical Variables

- region
- store_type

---

# Data Preparation

The original dataset was preserved.

Data preparation included:

- Checking missing values
- Verifying numerical data types
- Creating dummy variables
- Keeping original dataset unchanged
- Preparing data for regression

---

# Dummy Variable Approach

Dummy variables were created for Store Type.

Reference Category:

Retail Store

Remaining store types were converted into binary variables.

One category was omitted to prevent the Dummy Variable Trap.

---

# Regression Approach

The project includes:

Simple Regression Models

- Monthly Sales vs Marketing Spend
- Monthly Sales vs Footfall

Multiple Regression Model

Dependent Variable

- Monthly Sales

Independent Variables

- Marketing Spend
- Footfall
- Inventory Availability
- Customer Rating
- Store Type Dummy

---

# Model Comparison Summary

Simple regression models explain individual relationships.

The multiple regression model provides stronger explanatory power because it considers several operational drivers simultaneously.

---

# Final Model Selected

Multiple Linear Regression

Reason:

- Better explanatory power
- More realistic business interpretation
- Supports strategic decision making

---

# Business Recommendation

Leadership should prioritize:

- Increasing effective marketing spend
- Improving inventory availability
- Driving customer footfall
- Maintaining strong customer experience

Discount strategy should be interpreted carefully because excessive discounting may reduce profitability.

---

# Assumptions and Limitations

Regression identifies statistical association rather than causation.

Results may be affected by:

- Omitted variables
- Seasonal effects
- Economic conditions
- Promotional campaigns

---

# Screenshots Included

- simple_regression_output.png
- multiple_regression_output.png
- residuals_preview.png
- model_comparison_preview.png
