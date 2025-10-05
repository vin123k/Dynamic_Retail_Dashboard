# Dynamic Retail Dashboard

## Overview

This project involves the creation of a dynamic retail dashboard using Microsoft Excel, designed to visualize and analyze retail sales data across various dimensions. The dashboard connects to three main data tables—**Orders**, **Returns**, and **People**—and helps businesses gain insights into key sales performance metrics. This project is ideal for businesses looking to enhance their decision-making processes by analyzing data through dynamic visualizations and KPIs.

The dashboard includes key performance indicators (KPIs) that track important metrics such as **Total Sales**, **Total Profit**, **Quantity Sold**, **Number of Orders**, and **Profit Margin**. These KPIs are calculated and displayed on a centralized chart to ensure easy comparison and visualization. The project covers multiple problem statements that help break down the data into actionable insights.

---

## Sample Data Tables

### **Orders Table**
| Order ID         | Order Date | Ship Date  | Ship Mode    | Customer Name | Segment   | Country      | Sales   | Profit  | Quantity | Discount |
|------------------|------------|------------|--------------|---------------|-----------|--------------|---------|---------|----------|----------|
| CA-2012-124891   | 31-07-2020 | 31-07-2020 | Same Day     | Rick Hansen   | Consumer  | United States| 2309.65 | 762.18  | 7        | 0        |
| IN-2013-77878    | 05-02-2021 | 07-02-2021 | Second Class | Justin Ritter | Corporate | Australia    | 3709.40 | -288.77 | 9        | 0.1      |
| IN-2013-71249    | 17-10-2021 | 18-10-2021 | First Class  | Craig Reiter  | Consumer  | Australia    | 5175.17 | 919.97  | 9        | 0.1      |
| ES-2013-1579342  | 28-01-2021 | 30-01-2021 | First Class  | Katherine Murray | Home Office | Germany    | 2892.51 | -96.54  | 5        | 0.1      |
| SG-2013-4320     | 05-11-2021 | 06-11-2021 | Same Day     | Rick Hansen   | Consumer  | Senegal      | 2832.96 | 311.52  | 8        | 0        |

### **Return Table**
| Returned | Order ID         | Market     |
|----------|------------------|------------|
| Yes      | MX-2013-168137   | LATAM      |
| Yes      | US-2011-165316   | LATAM      |
| Yes      | ES-2013-1525878  | EU         |
| Yes      | CA-2013-118311   | United States |
| Yes      | ES-2011-1276768  | EU         |

### **People Table**
| Person            | Region  |
|-------------------|---------|
| Anna Andreadi     | Central |
| Chuck Magee       | South   |
| Kelly Williams    | East    |
| Matt Collister    | West    |
| Deborah Brumfield | Africa  |

---

## KPI Table

The KPI table consolidates the most essential performance metrics for the retail analysis. These KPIs allow the dashboard to provide actionable insights by comparing important aspects of sales performance.

| KPI Name          | Symbol | Formula                         |
|-------------------|--------|---------------------------------|
| Total Sales       | 💰     | SUM(Sales)                      |
| Total Profit      | 📈     | SUM(Profit)                     |
| Total Quantity    | 📦     | SUM(Quantity)                   |
| No of Orders      | 🛒     | COUNT(Order ID)                 |
| Profitability     | 🔍     | SUM(Profit) / SUM(Sales)        |

---

## Problem Statements Solved

The dynamic retail dashboard answers several business questions, providing in-depth insights into key performance areas:

1. **KPIs** - Total Sales, Total Profit, Quantity, No. of Orders, Profit Margin

![image](https://github.com/user-attachments/assets/9f9ce87e-8870-4d8c-818c-dc5696b15310)


2. **Sales and Profit Analysis** - Understanding overall sales and profitability

![image](https://github.com/user-attachments/assets/0a235d2b-86c0-4c3b-91c0-65c0e5c36d73)


3. **Category-wise Profit** - Breakdown of profit by product category

![image](https://github.com/user-attachments/assets/361c30ab-280b-4d27-9ca9-cb071b12fee2)


4. **Segment-wise Sales Share %** - Breakdown of sales by customer segment

![image](https://github.com/user-attachments/assets/7fa3ba5b-177f-40b8-8fa0-10f1e94c0cf9)


5. **Sales by Country** - Sales performance based on different countries

![image](https://github.com/user-attachments/assets/1074a818-8357-4a73-adf3-ae83c696eae7)


6. **Top 5 Subcategories** - The best-performing subcategories based on sales

![image](https://github.com/user-attachments/assets/9662c7c6-982f-4665-8e6a-93da8f46a481)


7. **Bottom 5 Subcategories** - The least-performing subcategories based on sales

![image](https://github.com/user-attachments/assets/b0be7e56-ce2f-4394-9519-0e2b751196a5)


8. **Yearly Sales Trend** - Understanding how sales evolve over the year

![image](https://github.com/user-attachments/assets/30f81444-e021-470f-b340-06bd41aa0e76)


---

## Snapshot of the Dashboard

![image](https://github.com/user-attachments/assets/fe996d48-4990-482b-986b-b3a7a654f749)

## Conclusion

The **Retail Dashboard** serves as an invaluable tool for business analysts and retail managers by providing a comprehensive view of sales performance. The dashboard aggregates data from key business areas and visualizes them dynamically, allowing for quick decision-making. With its ability to calculate essential KPIs and generate detailed analyses across different product categories, regions, and time periods, the dashboard ensures that stakeholders can make data-driven decisions to optimize retail operations.

