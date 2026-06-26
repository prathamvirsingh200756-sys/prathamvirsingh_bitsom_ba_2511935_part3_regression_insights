#  Regression Insights - Retail Sales Analysis

## Business Problem Summary
A retail chain's leadership team needs to understand what factors drive monthly sales performance across stores. They are considering various business actions including increasing marketing spend, improving inventory availability, changing discounting strategies, reallocating staff, and prioritizing certain store types or regions. This analysis uses regression techniques to identify which factors are most strongly associated with monthly sales.

## Dataset Description
The dataset `business_regression_data.xlsx` contains store-level monthly performance data with the following variables:

### Dependent Variable (Target)
- **monthly_sales** - Total monthly sales revenue ($)

### Potential Independent Variables

#### Numerical Variables:
- **marketing_spend** - Monthly marketing expenditure ($)
- **footfall** - Number of store visitors
- **avg_discount_pct** - Average discount percentage offered
- **inventory_availability_pct** - Percentage of products in stock
- **customer_rating** - Average customer satisfaction rating (1-5)
- **staff_count** - Number of employees
- **store_size_sqft** - Store size in square feet
- **avg_transaction_value** - Average value per transaction ($)

#### Categorical Variables:
- **region** - Store geographic region (North, South, East, West, Central)
- **store_type** - Type of store (Superstore, Express, Neighborhood, Mall)
- **weekend_footfall_ratio** - Ratio of weekend to weekday footfall

### Variables That May Need Cleaning or Transformation
1. **avg_discount_pct** - May need to check for outliers (stores with >50% discounts)
2. **inventory_availability_pct** - Should be between 0-100%; check for impossible values
3. **marketing_spend** - May need log transformation if highly skewed
4. **store_size_sqft** - Check for extreme values

### Variables That May Not Be Useful for Regression
1. **store_id** - This is just an identifier, not a predictor
2. **month** - Could be useful for time series analysis but in simple regression might not add value
3. **weekend_footfall_ratio** - May be highly correlated with footfall, causing multicollinearity

## Regression Approach

### Simple Regression Models
- Model 1: monthly_sales ~ marketing_spend
- Model 2: monthly_sales ~ footfall
- Additional models as needed

### Multiple Regression Model
- Model 3: monthly_sales ~ marketing_spend + footfall + avg_discount_pct + inventory_availability_pct + store_type_dummies + region_dummies

## Dummy Variable Approach
For categorical variables:
- **store_type**: Reference category = Express (most common store type)
- **region**: Reference category = Central (geographic center)

## Model Comparison Summary

| Model | Variables | R² | Significant Predictors |
|-------|-----------|----|---------------------|
| Simple Model 1 | marketing_spend | TBD | TBD |
| Simple Model 2 | footfall | TBD | TBD |
| Multiple Model | Multiple predictors | TBD | TBD |

## Final Model Selected
The final model will be selected based on highest adjusted R² and meaningful significant variables that provide actionable business insights.

## Business Recommendation
Leadership should focus on the variables that show the strongest statistical association with monthly sales while considering practical implementation constraints and cost-benefit analysis.

## Assumptions and Limitations
- Linearity assumption: Relationships between predictors and sales are linear
- Independence: Observations are independent
- Homoscedasticity: Constant variance of residuals
- Normality: Residuals are normally distributed
- No perfect multicollinearity among predictors

## Screenshots Included
- simple_regression_output.png - Shows simple regression output
- multiple_regression_output.png - Shows multiple regression output
- residuals_preview.png - Shows predicted values and residuals
- model_comparison_preview.png - Shows model comparison table
