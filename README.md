# 📊 Sales Analytics Dashboard | Power BI

## 📌 Project Overview

This project is an end-to-end Sales Analytics Dashboard developed in Power BI to analyze business performance across sales, products, customers, and returns.

The dashboard enables stakeholders to monitor key business metrics, identify trends, evaluate product performance, understand customer behavior, and make data-driven decisions through interactive visualizations and KPI tracking.

---

## 🎯 Business Objective

The primary objective of this dashboard is to:

- Monitor Revenue, Profit, Orders, and Return Rate.
- Track product performance and target achievement.
- Analyze customer purchasing behavior.
- Identify top-performing products and customers.
- Evaluate return trends and business growth.
- Support strategic decision-making through data visualization.

---

## 🛠️ Tools & Technologies Used

- Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Data Modeling
- Excel / CSV Data Sources

---

## 🏗️ Data Model

The dashboard follows a **Star Schema Data Model** consisting of Fact and Dimension tables.

### Fact Tables

#### Sales Data (2020–2022)
Contains transactional sales information including:

- Order Date
- Customer
- Product
- Quantity Ordered
- Revenue
- Profit
- Territory

#### Returns Data
Contains product return information including:

- Return Date
- Product Key
- Return Quantity
- Territory Key

### Dimension Tables

#### Calendar Lookup
Used for:
- Monthly Analysis
- Weekly Analysis
- Year-over-Year Reporting
- Time Intelligence

#### Customer Lookup
Contains:
- Customer Information
- Occupation
- Education
- Income Level

#### Product Lookup
Contains:
- Product Name
- Product SKU
- Product Price
- Product Cost
- Product Category

#### Product Categories Lookup
Contains product category hierarchy.

#### Product Subcategories Lookup
Contains product sub-category hierarchy.

#### Company Territory Lookup
Contains:
- Country
- Region
- Continent

---

## 📈 Dashboard Pages

### 1️⃣ Executive Dashboard

#### Key KPIs

| KPI | Value |
|------|--------|
| Revenue | $25M |
| Total Profit | $10M |
| Return Rate | 2% |
| Total Orders | 25K |

#### Visuals Included

- Monthly Revenue Trend
- Revenue Forecasting
- Orders by Category
- Top Products Analysis
- Return Analysis

#### Business Insights

- Accessories generated the highest order volume.
- Revenue showed steady growth throughout the reporting period.
- Return rate remained below 2%.
- Tires and Tubes emerged as the most ordered product category.

---

### 2️⃣ Product Analysis Dashboard

#### Key KPIs

- Orders vs Target
- Revenue vs Target
- Profit vs Target

#### Visuals Included

- Gauge Charts
- Product Performance Analysis
- Return Percentage Trend
- Monthly Product Metrics

#### Business Insights

- Mountain Tire Tube consistently achieved target performance.
- Product return percentage remained under control.
- Revenue and profit remained close to target values across most months.

---

### 3️⃣ Customer Analysis Dashboard

#### Key KPIs

| KPI | Value |
|------|--------|
| Unique Customers | 17K |
| Revenue per Customer | $1.43K |

#### Visuals Included

- Customer Trend Analysis
- Top Customers by Revenue
- Orders by Income Level
- Orders by Occupation
- Revenue per Customer Analysis

#### Business Insights

- Skilled customers generated the highest revenue contribution.
- Average income group contributed the highest order volume.
- Top customers generated significant revenue despite relatively fewer orders.

---

## 📊 Key Performance Indicators

### Revenue
Tracks total sales generated across all products.

### Profit
Tracks overall business profitability.

### Orders
Measures total number of customer orders.

### Return Rate
Tracks the percentage of returned products.

### Revenue Per Customer
Measures average revenue generated from each customer.

---

## 🧮 Sample DAX Measures

### Revenue

```DAX
Revenue =
SUM('Sales data 2020-2022'[Revenue])
```

### Profit

```DAX
Profit =
SUM('Sales data 2020-2022'[Profit])
```

### Total Orders

```DAX
Total Orders =
COUNTROWS('Sales data 2020-2022')
```

### Revenue Per Customer

```DAX
Revenue Per Customer =
DIVIDE(
    [Revenue],
    DISTINCTCOUNT('Customer Lookup'[CustomerKey])
)
```

### Return Rate

```DAX
Return Rate =
DIVIDE(
    [Returned Orders],
    [Total Orders]
)
```

---

## 📷 Dashboard Screenshots

### Executive Dashboard

<img width="1548" height="771" alt="Executive -Dashboard" src="https://github.com/user-attachments/assets/e7be4e1b-8f7b-4bc7-bcc2-80b150a531ad" />


### Product Analysis Dashboard

![Product Analysis Dashboard]<img width="1424" height="783" alt="Product-Analysis-Dashboard" src="https://github.com/user-attachments/assets/65407a53-aa06-42f8-a092-a8237e744f4d" />


### Customer Analysis Dashboard

![Customer Analysis Dashboard]<img width="1436" height="802" alt="Customer-Analysis-dashboard" src="https://github.com/user-attachments/assets/58afb2be-9512-4258-8e0a-12a3f5e05677" />


### Data Model

![Data Model]<img width="1768" height="809" alt="Data-Model" src="https://github.com/user-attachments/assets/4490c78b-43de-420a-ba00-a278ef82f466" />


---

## 🚀 Skills Demonstrated

- Power BI Dashboard Development
- Data Cleaning & Transformation
- Data Modeling (Star Schema)
- DAX Calculations
- KPI Design
- Forecasting
- Customer Analytics
- Product Analytics
- Return Analysis
- Business Intelligence Reporting
- Data Storytelling

---

## 📌 Project Outcome

Developed a comprehensive Business Intelligence solution that enables stakeholders to monitor sales performance, customer behavior, product effectiveness, and return trends through interactive and visually engaging dashboards.

The dashboard helps transform raw business data into meaningful insights for operational and strategic decision-making.

---

## 👩‍💻 Author

**Monika Gola**

Data Analyst | Power BI Developer

