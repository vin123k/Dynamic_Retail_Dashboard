# 🧭 Dynamic Retail Dashboard — Excel Module

## 📌 Project Overview
This project is a **Dynamic Retail Dashboard** built in **Microsoft Excel** for retail data analytics.  
It visualizes sales performance, profit trends, and return behavior using **interactive KPIs, PivotCharts, and slicers**.  
All datasets (`Orders`, `People`, `Returns`) were **ingested directly from GitHub** using **Power Query**.

---

## 📂 Data Sources
The dashboard is powered by **three key tables** stored on GitHub:

| Table Name | Description |
|-------------|--------------|
| **Orders** | Main transactional data containing sales, shipping, customer, and product details. |
| **People** | Regional manager assignments by region. |
| **Returns** | Order return details mapped by Order ID and Market. |

Additionally, a **KPI table** is used for displaying icons and metric labels in the dashboard.

---

## 🧾 Data Model

The relationship between tables is designed as follows:

- `Orders[Order ID]` → `Returns[Order ID]` *(one-to-many)*  
- `Orders[Region]` → `People[Region]` *(many-to-one)*  

These relationships allow insights like **returned orders by region**, **profit by manager**, and **sales by market**.

---

## 📊 Data Dictionary

### 🛍 Orders Table
| Column | Description |
|--------|--------------|
| **Order ID** | Unique identifier for each order |
| **Order Date** | Date when the order was placed |
| **Ship Date** | Date when the order was shipped |
| **Ship Mode** | Shipping method (e.g., Same Day, First Class) |
| **Customer ID** | Unique customer identifier |
| **Customer Name** | Full name of the customer |
| **Segment** | Customer type (Consumer, Corporate, Home Office) |
| **City / State / Country / Postal Code** | Geographic information |
| **Market** | Market name (e.g., US, EU, APAC) |
| **Region** | Regional classification |
| **Product ID** | Unique identifier for each product |
| **Category / Sub-Category / Product Name** | Product hierarchy details |
| **Sales** | Total sales amount |
| **Quantity** | Number of items sold |
| **Discount** | Discount applied (in %) |
| **Profit** | Net profit (may include negative values) |
| **Shipping Cost** | Cost incurred for shipping |
| **Order Priority** | Priority level (Critical, Medium, Low, etc.) |

---

### 👥 People Table
| Column | Description |
|--------|--------------|
| **Person** | Employee / Manager name |
| **Region** | Region assigned to that person |

This table is used to link each region with the responsible person or sales manager.

---

### 🔁 Returns Table
| Column | Description |
|--------|--------------|
| **Returned** | Indicates whether the order was returned (Yes/No) |
| **Order ID** | Order identifier that maps to the Orders table |
| **Market** | Market where the return occurred |

---

### 💡 KPI Table
| KPI | Name | Symbol |
|------|------|--------|
| Sum of Sales | Total Sales | 📈 |
| Sum of Profit | Total Profit | 💰 |
| Count of Order ID | Total Orders | 🛒 |
| Sum of Quantity | Total Quantity | 📦 |
| Sum of Profitability | Profitability | 🔍 |

---

## ⚙️ Tools & Technologies
- **Microsoft Excel** (with Power Query and Power Pivot)
- **Pivot Tables / Pivot Charts**
- **Data Model relationships**
- **GitHub (for CSV hosting & ingestion)**
- **Excel formulas and DAX measures**

---

## 🚀 Implementation Steps

### 1️⃣ Data Ingestion (via GitHub)
1. Go to **Data → Get Data → From Web**  
2. Paste the **Raw GitHub URL** for each dataset (`Orders`, `People`, `Returns`).  
3. Use **Power Query Editor** to:
   - Promote headers  
   - Change data types  
   - Remove blank rows or duplicates  
   - Ensure correct date format (`dd-mm-yyyy`)

4. Load the cleaned tables into the **Data Model** (`Close & Load To → Only Create Connection + Add to Data Model`).

---

### 2️⃣ Create Relationships
In **Power Pivot → Diagram View**:
- Link `Orders[Order ID]` → `Returns[Order ID]`
- Link `Orders[Region]` → `People[Region]`

This ensures consistent lookups for region-based analysis and return rates.

---

### 3️⃣ Build DAX Measures
Create the following **calculated measures** inside the Data Model:

```DAX
Total Sales := SUM(Orders[Sales])
Total Profit := SUM(Orders[Profit])
Total Quantity := SUM(Orders[Quantity])
Total Orders := DISTINCTCOUNT(Orders[Order ID])
Profitability := DIVIDE([Total Profit], [Total Sales], 0)

Returned Orders := DISTINCTCOUNT(Returns[Order ID])
Return Rate := DIVIDE([Returned Orders], [Total Orders], 0)

