# DAX Measures

This document contains the core DAX measures used in the FMCG Sales Analytics Power BI project.

---

## 1. Core Sales & Revenue Measures

### Total Gross Sales

**Purpose:** Calculates total sales revenue before discounts.

```DAX
Total Gross Sales =
SUM(fact_sales[SalesAmount])
```

### Total Discount

**Purpose:** Calculates the total monetary discount applied to sales.

```DAX
Total Discount =
SUM(fact_sales[DiscountAmount])
```

### Total Net Revenue

**Purpose:** Calculates revenue after deducting discounts from gross sales.

```DAX
Total Net Revenue =
[Total Gross Sales] - [Total Discount]
```

### Total Cost

**Purpose:** Calculates the total cost associated with sold products.

```DAX
Total Cost =
SUM(fact_sales[TotalCost])
```

### Total Gross Profit

**Purpose:** Calculates gross profit after deducting total cost from net revenue.

```DAX
Total Gross Profit =
[Total Net Revenue] - [Total Cost]
```

---

## 2. Profitability Measures

### Profit Margin %

**Purpose:** Measures gross profit as a percentage of net revenue.

```DAX
Profit Margin % =
DIVIDE(
    [Total Gross Profit],
    [Total Net Revenue],
    0
)
```

### Discount Rate %

**Purpose:** Measures the percentage of gross sales given as discounts.

```DAX
Discount Rate % =
DIVIDE(
    [Total Discount],
    [Total Gross Sales],
    0
)
```

---

## 3. Volume & Order Measures

### Total Orders

**Purpose:** Counts the number of unique sales orders.

```DAX
Total Orders =
DISTINCTCOUNT(fact_sales[SalesOrderNumber])
```

### Total Quantity

**Purpose:** Calculates the total number of units sold.

```DAX
Total Quantity =
SUM(fact_sales[Quantity])
```

### AOV

**Purpose:** Calculates the average net revenue generated per order.

```DAX
AOV =
DIVIDE(
    [Total Net Revenue],
    [Total Orders],
    0
)
```

---

## 4. Order Status Measures

### Delivered Orders

**Purpose:** Counts orders with a Delivered status.

```DAX
Delivered Orders =
CALCULATE(
    [Total Orders],
    fact_sales[OrderStatus] = "Delivered"
)
```

### Cancelled Orders

**Purpose:** Counts orders with a Cancelled status.

```DAX
Cancelled Orders =
CALCULATE(
    [Total Orders],
    fact_sales[OrderStatus] = "Cancelled"
)
```

### Returned Orders

**Purpose:** Counts orders with a Returned status.

```DAX
Returned Orders =
CALCULATE(
    [Total Orders],
    fact_sales[OrderStatus] = "Returned"
)
```

### Spoiled Orders

**Purpose:** Counts orders with a Spoiled status.

```DAX
Spoiled Orders =
CALCULATE(
    [Total Orders],
    fact_sales[OrderStatus] = "Spoiled"
)
```

### Non Delivered Orders

**Purpose:** Counts all orders that were not delivered.

```DAX
Non Delivered Orders =
CALCULATE(
    [Total Orders],
    fact_sales[OrderStatus] <> "Delivered"
)
```

### Non Delivered Rate %

**Purpose:** Measures the percentage of total orders that were not delivered.

```DAX
Non Delivered Rate % =
DIVIDE(
    [Non Delivered Orders],
    [Total Orders],
    0
)
```

---

## 5. Non-Delivered Revenue Measures

### Non Delivered Revenue

**Purpose:** Calculates net revenue associated with orders that were not delivered.

```DAX
Non Delivered Revenue =
CALCULATE(
    [Total Net Revenue],
    fact_sales[OrderStatus] <> "Delivered"
)
```

### Non Delivered Revenue %

**Purpose:** Measures the percentage of total net revenue associated with non-delivered orders.

```DAX
Non Delivered Revenue % =
DIVIDE(
    [Non Delivered Revenue],
    [Total Net Revenue],
    0
)
```

---

## 6. Year-over-Year Measures

### Net Revenue LY

**Purpose:** Calculates net revenue for the equivalent period in the previous year.

```DAX
Net Revenue LY =
CALCULATE(
    [Total Net Revenue],
    SAMEPERIODLASTYEAR(dim_calender[Date])
)
```

### YoY Growth

**Purpose:** Calculates the absolute change in net revenue compared with the previous year.

```DAX
YoY Growth =
[Total Net Revenue] - [Net Revenue LY]
```

### YoY Growth %

**Purpose:** Calculates the percentage change in net revenue compared with the previous year.

```DAX
YoY Growth % =
DIVIDE(
    [YoY Growth],
    [Net Revenue LY],
    0
)
```

---

## 7. Measure Summary

| Measure                 | Category      | Description                            |
| ----------------------- | ------------- | -------------------------------------- |
| Total Gross Sales       | Revenue       | Gross sales before discounts           |
| Total Discount          | Revenue       | Total monetary discounts               |
| Total Net Revenue       | Revenue       | Revenue after discounts                |
| Total Cost              | Cost          | Total product cost                     |
| Total Gross Profit      | Profitability | Net revenue minus cost                 |
| Profit Margin %         | Profitability | Gross profit as % of net revenue       |
| Discount Rate %         | Profitability | Discount as % of gross sales           |
| Total Orders            | Orders        | Number of unique orders                |
| Total Quantity          | Volume        | Total units sold                       |
| AOV                     | Orders        | Average revenue per order              |
| Delivered Orders        | Order Status  | Delivered orders                       |
| Cancelled Orders        | Order Status  | Cancelled orders                       |
| Returned Orders         | Order Status  | Returned orders                        |
| Spoiled Orders          | Order Status  | Spoiled orders                         |
| Non Delivered Orders    | Order Status  | Orders not delivered                   |
| Non Delivered Rate %    | Order Status  | % of orders not delivered              |
| Non Delivered Revenue   | Revenue       | Revenue from non-delivered orders      |
| Non Delivered Revenue % | Revenue       | % of revenue from non-delivered orders |
| Net Revenue LY          | YoY           | Previous-year net revenue              |
| YoY Growth              | YoY           | Absolute revenue change                |
| YoY Growth %            | YoY           | Percentage revenue change              |

---
