# FMCG Sales & Profitability Analytics — Power BI

> **Turning transactional FMCG data into actionable commercial insights**

![Power BI](https://img.shields.io/badge/Power%20BI-Analytics-F2C811?logo=powerbi\&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Measures-1F4E79)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-68217A)
![Data Modeling](https://img.shields.io/badge/Data%20Model-Star%20Schema-2E7D32)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 📊 Project Overview

This project is an end-to-end **FMCG Sales & Profitability Analytics solution built in Power BI**.

The goal was to transform transactional sales data into a business intelligence solution that helps commercial and sales teams understand:

* Revenue and profitability performance
* Year-over-Year performance
* Monthly and quarterly trends
* Category and SKU contribution
* Customer and channel performance
* Geographic opportunities
* Promotion effectiveness
* Discount impact on profitability
* Operational issues
* Drivers behind revenue decline

The analysis compares **2024 performance against 2023** and translates the results into actionable business recommendations.

---

# 🎯 Business Objective

The project aims to answer a fundamental business question:

> **How can the business recover revenue growth while protecting the profitability improvements achieved in 2024?**

To answer this, the analysis focuses on five areas:

1. **Growth** — Where did revenue increase or decline?
2. **Profitability** — Which products, channels and customers generate profitable revenue?
3. **Commercial effectiveness** — Are promotions and discounts creating value?
4. **Customer & market performance** — Where should sales teams focus?
5. **Operational performance** — Are returns, cancellations and non-deliveries materially affecting results?

---

# 🧩 Business Questions

The Power BI report was designed around the following questions:

1. How did we perform YoY?
2. Which months drove growth or decline?
3. Which categories drive sales and profit?
4. Which SKUs need attention?
5. Which channels perform best?
6. Which customers matter most?
7. Where is performance strongest?
8. Are promotions effective?
9. Is discount hurting margin?
10. Are operational issues material?
11. What drove growth or decline?

---

# 📈 Executive Findings

## 1. YoY Performance

Net Revenue declined **11.69% YoY**, from **296.49M in 2023 to 261.82M in 2024**, following a **14.40% decline in Gross Sales**.

However, Gross Profit declined by only **3.07%**, while Gross Margin improved from **26.73% to 29.35%**, representing a **+2.62 percentage-point improvement**.

### Business Interpretation

The business experienced a significant top-line contraction, but profitability was relatively protected.

This suggests that stronger commercial discipline helped offset part of the impact of lower sales.

---

## 2. Monthly Performance

Net Revenue remained relatively stable during **January–April 2024**, at approximately **24M–24.5M per month**, while Gross Margin remained around **26.6%**.

From June onward, the effective discount rate declined while Gross Margin improved significantly to approximately **32%** and remained relatively strong through December.

### Business Interpretation

The second half of 2024 shows a shift toward **margin protection and lower discount dependency**, even though monthly revenue remained lower.

---

## 3. Category Performance

### Home Care

* Highest Gross Profit: **43.8M**
* Lowest Gross Margin: **24.93%**

Home Care is the largest profit contributor but has significant margin optimization potential.

### Personal Care

* Highest Gross Margin: **31.37%**

Personal Care represents a strong profitability benchmark.

### Beverages

* Highest sales volume: **5.07M units**
* Gross Margin: **30.97%**

Beverages combine high volume with strong profitability.

### Packaged Food

* Gross Profit: **32.0M**
* Gross Margin: **29.83%**

Packaged Food also demonstrates a strong profitability profile.

### Business Interpretation

The category generating the most Gross Profit is not necessarily the category with the highest margin.

This highlights the importance of analyzing both:

**Profit contribution + Profitability rate**

---

# 🏷️ SKU Analysis

## Priority SKU: Ariel Automatic Gel 2L

Ariel Automatic Gel 2L is:

* The highest-revenue SKU
* The highest-profit SKU
* Operating at a relatively low **24.93% Gross Margin**
* Carrying the highest discount rate at **6.39%**

### Recommendation

Because of its commercial importance, pricing and discounting should be reviewed carefully without disrupting its high sales contribution.

---

## Other SKUs Requiring Attention

### Juhayna Full Cream Milk

* Lowest Gross Margin: **23.19%**

Requires investigation into:

* Pricing
* Cost structure
* Discounting
* Product mix

### El-Arousa Black Tea

Combines:

* High revenue
* Below-average margin
* Above-average discounting

This makes it another candidate for commercial review.

---

# 🛒 Channel Performance

Traditional Trade and Modern Trade are the strongest channels.

Together they contribute approximately:

* **55% of Revenue**
* **56% of Gross Profit**

while maintaining margins around **28.3%**.

Their discount rates are approximately **5.6%**.

By comparison:

* E-Commerce
* Cash & Carry

operate with lower margins and higher discount rates of approximately **6.49%**.

### Business Interpretation

Channel performance should not be evaluated by revenue alone.

The key question is:

> **Which channels generate profitable growth?**

---

# 👥 Customer Analysis

### Revenue Leader

**Hyper One — Branch #29**

was among the leading customers by Revenue.

### Profit Leader

**Kazyon Market — Branch #49**

was among the leading customers by Gross Profit.

### Margin Concern

Gourmet Egypt branches showed strong sales contribution but comparatively compressed margins.

### Recommendation

High-value accounts should be segmented into:

* High Revenue / High Margin
* High Revenue / Low Margin
* Low Revenue / High Margin
* Low Revenue / Low Margin

This allows the sales team to prioritize accounts based on both commercial value and profitability.

---

# 📍 Geographic Performance

### Cairo

Strongest market by:

* Revenue
* Gross Profit

### Giza

Highest Gross Margin.

### Beheira & Sharqia

Generate meaningful revenue and represent potential areas for:

* Additional sales coverage
* Distribution expansion
* Customer acquisition
* Growth investigation

---

# 🎁 Promotion Effectiveness

Promotion performance varies significantly.

### Strong Promotions

**Buy 10 Cases Get 1 Free**

and

**End of Month Volume Rebate**

generate strong commercial contribution while maintaining relatively healthy margins.

### Promotion Requiring Review

**Back to School Flash Promo**

* Gross Margin: **15.32%**
* Discount Rate: **20%**

This promotion represents a significant margin risk.

### Recommendation

Promotions should be evaluated using:

**Sales + Volume + Gross Profit + Gross Margin + Discount**

rather than sales uplift alone.

---

# 💸 Discount Impact

The effective discount rate declined from:

**7.38% → 4.45%**

between 2023 and 2024.

This resulted in:

* **48.35% reduction in total discount spend**
* **+2.62 percentage-point improvement in Gross Margin**

### Business Interpretation

Stronger discount discipline coincided with materially improved margin performance.

> This is an observed relationship in the dataset and should not automatically be interpreted as causal without further statistical testing.

---

# ⚠️ Operational Performance

Non-delivered orders represent a significant share of total order activity.

Returned, Cancelled and Spoiled orders therefore require further financial assessment.

The next analytical step would be to quantify:

* Lost Revenue
* Lost Gross Profit
* Returned Quantity
* Return Rate
* Cancellation Rate
* Spoilage impact

and identify whether these issues are concentrated by:

* Product
* Customer
* Channel
* Geography

---

# 🔎 What Drove the Revenue Decline?

The decline in Net Revenue was primarily associated with:

* Lower sales volume
* Fewer orders

However:

* Improved price realization
* Lower discount rates

helped protect Gross Margin and limited the decline in Gross Profit.

### Executive Conclusion

The 2024 problem was primarily a **top-line / volume problem**, rather than an equivalent collapse in profitability.

This leads to the central management question:

> **How can the business recover volume while maintaining the margin discipline achieved in 2024?**

---

# 🏗️ Data Architecture

The project follows a dimensional/star-schema approach.

## Fact Tables

### Fact_Sales

Contains transaction-level sales data.

---

## Dimension Tables

### Dim_Calendar

Provides:

* Date
* Year
* Quarter
* Month
* Month Number
* Year-Month

and supports DAX time intelligence.

### Dim_Customers

Contains customer/account attributes.

### Dim_Products

Contains SKU and category attributes.

### Dim_Channels

Contains sales channel attributes.

### Dim_Promotions

Contains promotion and campaign attributes.

---

## Model Structure

```text
                         Dim_Calendar
                              |
                              |
Dim_Customers ----->     Fact_Sales     <----- Dim_Products
Dim_Promotions ----->
                              |
                              |
                        Dim_Channels
                        
```

The model uses **one-to-many relationships from dimensions to fact tables**.

This allows dimensions such as Product, Customer, Channel and Promotion to filter sales consistently.

---

# 🧮 DAX Measures

The project uses reusable DAX measures rather than relying exclusively on implicit aggregations.

## Total Sales

```DAX
Total Sales :=
SUM(Fact_Sales[Sales_Amount])
```

## Total Cost

```DAX
Total Cost :=
SUM(Fact_Sales[Total_Cost])
```

## Gross Profit

```DAX
Gross Profit :=
[Total Sales] - [Total Cost]
```

## Gross Margin %

```DAX
Gross Margin % :=
DIVIDE(
    [Gross Profit],
    [Total Sales]
)
```

## Total Quantity

```DAX
Total Quantity :=
SUM(Fact_Sales[Quantity])
```

## Orders

```DAX
Orders :=
DISTINCTCOUNT(Fact_Sales[Order_ID])
```

## Customers

```DAX
Customers :=
DISTINCTCOUNT(Fact_Sales[Customer_ID])
```

## Sales LY

```DAX
Sales LY :=
CALCULATE(
    [Total Sales],
    SAMEPERIODLASTYEAR(Dim_Calendar[Date])
)
```

## Sales YoY

```DAX
Sales YoY :=
[Total Sales] - [Sales LY]
```

## Sales YoY %

```DAX
Sales YoY % :=
DIVIDE(
    [Sales YoY],
    [Sales LY]
)
```

## Profit LY

```DAX
Profit LY :=
CALCULATE(
    [Gross Profit],
    SAMEPERIODLASTYEAR(Dim_Calendar[Date])
)
```

## Profit YoY %

```DAX
Profit YoY % :=
DIVIDE(
    [Gross Profit] - [Profit LY],
    [Profit LY]
)
```

## Return Rate

```DAX
Return Rate :=
DIVIDE(
    [Returned Quantity],
    [Total Quantity]
)
```

> The exact column and measure names should match the final Power BI model.

---

# 📊 Power BI Report Structure

## Page 1 — Executive Overview

Focus:

* Revenue
* YoY performance
* Gross Profit
* Gross Margin
* Orders
* Quantity
* Customers
* Return Rate
* Monthly trend
* Category contribution
* Channel performance
* Top SKUs

---

## Page 2 — Sales & Profitability

Focus:

* Monthly YoY
* Quarterly YoY
* Revenue
* Gross Profit
* Gross Margin
* Category performance
* SKU performance
* Volume
* Discount impact

---

## Page 3 — Customers, Channels & Promotions

Focus:

* Customer performance
* Customer segmentation
* Channel profitability
* Geographic performance
* Promotion effectiveness
* Discount analysis
* High-value / low-margin accounts

---

# 💡 Key Recommendations

### 1. Recover Volume Without Reintroducing Excessive Discounting

Revenue declined primarily because of lower volume and fewer orders.

The priority should therefore be volume recovery while maintaining the improved discount discipline achieved in 2024.

### 2. Review High-Revenue / Low-Margin SKUs

Prioritize products such as:

* Ariel Automatic Gel 2L
* Juhayna Full Cream Milk
* El-Arousa Black Tea

for pricing, cost and discount analysis.

### 3. Optimize Promotion Strategy

Maintain promotions that generate commercial value without severe margin erosion.

Review or redesign promotions with excessive discounts and weak margins.

### 4. Focus on Profitable Channels

Traditional Trade and Modern Trade demonstrate strong scale and healthy profitability.

Lower-margin channels should be evaluated based on their incremental commercial contribution.

### 5. Protect Strategic Customers

Identify accounts with:

* High Revenue
* High Profit
* High Growth

while separately monitoring:

* High Revenue
* Low Margin

customers.

### 6. Investigate Regional Growth Opportunities

Maintain focus on Cairo and Giza while investigating expansion opportunities in Beheira and Sharqia.

### 7. Quantify Operational Leakage

Measure the actual financial impact of:

* Returns
* Cancellations
* Spoilage
* Non-deliveries

to determine whether operational issues materially contribute to lost profitability.

---

# 🛠️ Tools & Skills Demonstrated

## Power BI

* Power Query
* Data Transformation
* Data Modeling
* Star Schema
* Relationships
* DAX
* Time Intelligence
* Interactive Dashboards
* KPI Design
* Drill-down Analysis
* Business Storytelling

## Analytics

* YoY Analysis
* Trend Analysis
* Profitability Analysis
* Margin Analysis
* SKU Analysis
* Customer Analysis
* Channel Analysis
* Promotion Analysis
* Discount Analysis
* Operational Analysis
* Driver Analysis

## Business

* Revenue Management
* Margin Protection
* Pricing Analysis
* Promotion Optimization
* Customer Prioritization
* Channel Strategy
* Commercial Decision Support

---

# 📁 Repository Structure

```text
FMCG-Sales-Profitability-PowerBI/
│
├── README.md
│
├── PowerBI/
│   └── FMCG_Sales_Analytics.pbix
│
├── Documentation/
│   ├── Data_Dictionary.xlsx
│   ├── DAX_Measures.md
│   ├── Business_Questions.md
│   └── Data_Model.png
│
├── Screenshots/
│   ├── 01_Executive_Overview.png
│   ├── 02_Sales_Profitability.png
│   └── 03_Customers_Promotions.png
│
├── Data/
│   └── README.md
│
└── .gitignore
```

---

# 🚀 Project Outcome

This project demonstrates a complete business intelligence workflow:

```text
Raw Transactional Data
        ↓
Data Cleaning
        ↓
Data Validation
        ↓
Dimensional Modeling
        ↓
DAX Measures
        ↓
Business Analysis
        ↓
Insights
        ↓
Recommendations
        ↓
Power BI Dashboard
```

The final analysis shows that:

> **2024 experienced an 11.69% decline in Net Revenue, primarily driven by lower volume and fewer orders. However, improved price realization and substantially lower discounting protected profitability, resulting in only a 3.07% decline in Gross Profit while Gross Margin improved by 2.62 percentage points.**

The key business opportunity is therefore not simply to increase sales, but to **recover profitable volume while preserving the margin discipline established during 2024**.

---

# 👤 Author

## Ahmed Adel

**Aspiring Data Analyst | Power BI | SQL | Excel | Python**

This project was developed as a portfolio case study demonstrating practical skills in data cleaning, dimensional modeling, DAX, business analysis, visualization and data-driven decision making.

