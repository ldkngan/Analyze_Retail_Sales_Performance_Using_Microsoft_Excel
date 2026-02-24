# Analyze Retail Sales Performance Using Microsoft Excel
<img width="1200" height="675" alt="excel bicycle sales performance" src="https://github.com/user-attachments/assets/f7056231-0890-440a-8994-271b7f54dde3" />

This project analyzes sales performance of a global bicycle retail company using Excel. It converts raw transactional data into a structured data model and interactive dashboard, enabling management to track revenue, profit, regional performance, customer segments, and discount impact to support strategic planning for the next business cycle.
- **Author:** Le Dang Kim Ngan
- **Tool Used:** Microsoft  Excel (Power Query, Power Pivot, Pivot Tables)

---

## 📋 Table of Contents
1. Overview
2. Introduction to Dataset
3. Design Thinking Process
4. Visualization & Key Insights
5. Recommendations

---

## ✨ Overview
### 🏢 Business Context
This project analyzes **sales performance** of a **global retail bicycle company** operating across multiple countries and continents. The company sells various bicycle products to different customer segments and applies discount strategies to compete in a highly competitive retail market.

However, raw data alone does not provide clear insights into:
- Profitability trends
- Regional performance gaps
- Effectiveness of discount strategies
- Customer segment contribution to revenue

Management needs a centralized reporting system to support data-driven strategic planning for the next fiscal year.

### 🎯 Project Objective
The main objective of this project is to build an **interactive Excel Dashboard** that enables the CEO and Directors to:
- Review overall sales performance over the past years
- Monitor revenue, cost, and profit trends
- Evaluate performance by product, region, and customer segment
- Assess the impact of discount strategies on profitability
- Identify underperforming areas and growth opportunities
- Support strategic planning and budgeting for the upcoming year

### 🔖 Key Business Questions
1. How has total revenue and profit evolved over time (monthly, yearly)?
2. Which products contribute the most to revenue and profit?
3. Which regions or countries are driving growth, and which are underperforming?
4. Which customer segments generate the highest value?
5. How do discount rates impact overall profitability?
6. Where should the company focus its strategy for the next year to maximize growth and margin?

---

## 📂 Introduction to Dataset
<details>
<summary>The dataset consists of six tables structured in a dimensional data model</summary>

| Table | Description |
|-------|-------------|
| **fact_sale_2020-2021** | Central fact table containing transactional sales data: order date, product, customer, segment, region, discount rate, units sold, and sale price |
| **dim_date** | Stores calendar attributes such as year, month, month-year, and day of week to support time-based analysis |
| **dim_product** | Contains product details including product name and manufacturing price |
| **dim_customer** | Stores customer-level information |
| **dim_customer_segment** | Defines customer segmentation categories |
| **dim_region** | Provides geographic information including country and continent |

</details>

**Data Relationships:**
- This project applies a **star schema** model.
- The **fact_sale_2020-2021** table serves as the central fact table and connects to all dimension tables through **one-to-many** relationships.

This structure enables efficient slicing and dicing of sales performance by time, product, customer segment, and geography, supporting multi-dimensional business analysis.

<img width="1358" height="674" alt="image" src="https://github.com/user-attachments/assets/e0927965-3427-4ac9-98cb-4f8d9ba65af1" />


---

## 🧠 Design Thinking Process
<img width="1015" height="578" alt="image" src="https://github.com/user-attachments/assets/071f964c-2824-49be-8337-95fa22397627" />

---

## 📊 Visualization & Key Insights
<img width="1342" height="716" alt="image" src="https://github.com/user-attachments/assets/7a77bdfa-7119-4e9a-921e-1b5dc1edad64" />

### Key Insights

- Revenue reached **355.12M** with **49.36% profit margin**, showing strong growth YoY, mainly driven by higher sales volume rather than margin expansion.
- Clear **seasonality pattern**, with revenue peaks in mid-year and Q4; margin dips in some periods suggest discount impact.
- **Government segment contributes 42% of total revenue** → high customer concentration risk.
- **England (55.5 M) and Japan (53.6 M) are top-performing markets**, with relatively balanced revenue distribution across countries.
- **X-Terrain and Yellow Edition are key profit drivers**, while heavy discounts (e.g., City Cruiser) do not necessarily translate into higher profit.
- Revenue is concentrated in a few top products → opportunity to optimize pricing strategy and improve performance of lower-tier SKUs.

---

## 🚀 Recommendations
| Strategic Focus                | Key Recommendation                                                                                                                   | Expected Impact                                  |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------ |
| Profit Margin Optimization     | Review product-level discount strategy; shift from volume-driven to margin-based pricing; closely monitor monthly margin fluctuation | Improve profitability and prevent margin erosion |
| Scale Top Markets              | Prioritize investment in **England (55.5M)** and **Japan (53.6M)**; replicate successful sales strategies to other regions           | Accelerate growth in high-performing markets     |
| Revenue Diversification        | Reduce reliance on Government segment (42% revenue); strengthen Enterprise & Small Business acquisition                              | Lower customer concentration risk                |
| Product Portfolio Optimization | Focus on high-margin products (X-Terrain, Yellow Edition); reassess pricing and positioning of low-performing SKUs                   | Improve overall product mix performance          |
| Seasonal Strategy Planning     | Increase inventory & marketing before peak periods (mid-year, Q4); limit aggressive discounting in off-peak months                   | Maximize peak revenue while protecting margin    |
