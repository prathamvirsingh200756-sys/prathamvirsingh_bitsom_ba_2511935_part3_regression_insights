# Regression Model Equations

## Simple Regression 1

Monthly Sales = β₀ + β₁(Marketing Spend)

Interpretation

β₁ represents the expected change in monthly sales for each additional unit of marketing spend.

---

## Simple Regression 2

Monthly Sales = β₀ + β₁(Footfall)

Interpretation

β₁ represents the increase in monthly sales associated with additional customer visits.

---

## Multiple Regression

Monthly Sales = β₀
+ β₁(Marketing Spend)
+ β₂(Footfall)
+ β₃(Inventory Availability)
+ β₄(Customer Rating)
+ β₅(Store Type Dummy)

---

## Dummy Variables

Store Type

Reference Category

Retail Store

Dummy Variable

Outlet Store

Outlet = 1

Retail = 0

This avoids perfect multicollinearity.

---

## Coefficient Interpretation

Marketing Spend

Higher marketing investment is expected to increase sales.

Footfall

More visitors generally produce higher sales.

Inventory Availability

Better stock availability supports increased sales.

Customer Rating

Higher customer satisfaction is associated with stronger sales.

Store Type Dummy

Measures the average sales difference between outlet stores and the reference retail stores.

---

## Final Model

Selected Model

Multiple Linear Regression

Reason

- Uses multiple business drivers
- Stronger explanatory capability
- Better suited for strategic decision making
