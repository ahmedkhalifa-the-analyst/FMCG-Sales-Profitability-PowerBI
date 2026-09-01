# Data Cleaning & Validation

## 1. Data Preparation

The dataset was reviewed and prepared before being loaded into Power BI to ensure data quality, consistency, and reliability of the analysis.

The preparation process included:

* Reviewing table structures and column data types
* Checking for missing values
* Checking for duplicate records
* Validating relationships between fact and dimension tables
* Standardizing categorical values
* Validating dates and numeric fields
* Checking business rules and calculated values
* Validating the final dataset before analysis

---

## 2. Data Quality Checks

### Missing Values

Checked important fields across the dataset for missing values, including:

* Customer identifiers
* Product identifiers
* Order dates
* Order status
* Promotion identifiers
* Numeric sales fields

Missing values were investigated and handled according to the project's business rules.

---

### Duplicate Records

The dataset was checked for duplicate transaction records and duplicate dimension keys.

Primary keys in the dimension tables were validated to ensure uniqueness.

---

### Data Types

Column data types were reviewed and standardized.

Examples include:

* Dates → Date
* Quantities → Whole Number
* Prices and costs → Decimal Number
* Discount percentages → Decimal Number
* IDs → Text

---

### Categorical Standardization

Categorical fields were reviewed for inconsistent values and standardized to ensure consistent filtering and aggregation in Power BI.

Examples include:

* Product categories
* Order status
* Customer segments
* Sales channels
* Geographic fields

---

## 3. Business Rule Validation

The final dataset was validated against the project's business rules.

Key checks included:

* Quantity must be greater than zero.
* Sales Amount must be greater than zero.
* Order Date must contain a valid date.
* Customer and Product IDs must exist in their respective dimension tables.
* Promotion IDs must exist in the promotion dimension.
* Dimension primary keys must be unique.
* Order Status must contain a valid business status.

---

## 4. Financial Validation

Sales and profitability calculations were validated to ensure consistency between the underlying fields and the Power BI measures.

### Gross Sales

Gross Sales is calculated as:

```text
Gross Sales = Sales Amount
```

### Net Revenue

Net Revenue is calculated as:

```text
Net Revenue = Gross Sales - Discount Amount
```

### Gross Profit

Gross Profit is calculated as:

```text
Gross Profit = Net Revenue - Total Cost
```

### Gross Margin

Gross Margin is calculated as:

```text
Gross Margin % = Gross Profit / Net Revenue
```

These calculations were cross-checked against aggregated results to validate the financial logic used in the Power BI model.

---

## 5. Data Model Validation

The final dataset was structured using a star schema.

The `Fact_Sales` table is connected to the following dimension tables:

* `Dim_Calendar`
* `Dim_Products`
* `Dim_Customers`
* `Dim_Channels`
* `Dim_Promotions`

Relationships were validated to ensure that fact-table foreign keys correctly map to the corresponding dimension keys.

---

## 6. Final Validation

After cleaning and transformation, the dataset was reviewed again to confirm:

* No unexpected duplicate dimension keys
* Valid fact-to-dimension relationships
* Valid dates and numeric values
* Consistent categorical values
* Correct financial calculations
* Consistent Power BI measures

The validated dataset was then used as the source for the Power BI analysis and dashboard.

---

## Outcome

The data preparation and validation process established a consistent and analysis-ready dataset, providing a reliable foundation for the Power BI data model, DAX calculations, and business insights.
