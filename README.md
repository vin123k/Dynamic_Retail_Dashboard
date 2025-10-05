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

<img width="866" height="101" alt="Screenshot 2025-10-05 180157" src="https://github.com/user-attachments/assets/4a31515e-f320-49d8-82da-64d79a47d9aa" />

2. **Sales and Profit Analysis** - Understanding overall sales and profitability

<img width="370" height="285" alt="Screenshot 2025-10-05 180415" src="https://github.com/user-attachments/assets/17f0d956-5634-40be-bf49-92c1283f74f3" />

3. **Category-wise Profit** - Breakdown of profit by product category

<img width="274" height="282" alt="Screenshot 2025-10-05 180604" src="https://github.com/user-attachments/assets/80efa549-49b1-43bf-b87f-cdf3e472e2e5" />

4. **Segment-wise Sales Share %** - Breakdown of sales by customer segment

<img width="286" height="276" alt="Screenshot 2025-10-05 180642" src="https://github.com/user-attachments/assets/85a0d889-805e-4887-9c3c-4de8c0baf4ab" />

5. **Sales by Country** - Sales performance based on different countries

<img width="379" height="280" alt="Screenshot 2025-10-05 180701" src="https://github.com/user-attachments/assets/b1cb5589-cf07-4dc1-a1ce-530a37c1e3dc" />

6. **Top 5 Subcategories** - The best-performing subcategories based on sales

<img width="293" height="269" alt="Screenshot 2025-10-05 180445" src="https://github.com/user-attachments/assets/20425cac-7c99-4e11-b72d-fe6102d93149" />

7. **Bottom 5 Subcategories** - The least-performing subcategories based on sales

<img width="330" height="284" alt="Screenshot 2025-10-05 180431" src="https://github.com/user-attachments/assets/21487b83-3ff8-44c8-8d5a-b34a6ef14e25" />

8. **Yearly Sales Trend** - Understanding how sales evolve over the year

<img width="869" height="165" alt="Screenshot 2025-10-05 180728" src="https://github.com/user-attachments/assets/52c7db80-5082-4356-a183-f522066fc71c" />

---

## Snapshot of the Dashboard

<img width="1386" height="582" alt="Screenshot 2025-10-05 180834" src="https://github.com/user-attachments/assets/46dc7509-e15f-4d90-8a18-a3fd577f473e" />

## Conclusion

The **Retail Dashboard** serves as an invaluable tool for business analysts and retail managers by providing a comprehensive view of sales performance. The dashboard aggregates data from key business areas and visualizes them dynamically, allowing for quick decision-making. With its ability to calculate essential KPIs and generate detailed analyses across different product categories, regions, and time periods, the dashboard ensures that stakeholders can make data-driven decisions to optimize retail operations.

