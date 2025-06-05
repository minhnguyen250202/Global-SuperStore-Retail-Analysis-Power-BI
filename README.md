![image](https://github.com/user-attachments/assets/58aa2228-543a-4a5c-93b1-78e4f5b1c228)# 📊 Global-SuperStore-Retail-Analysis-Power-BI

<img width="952" alt="image" src="https://github.com/user-attachments/assets/19979350-1c9e-475e-b174-b9b6267a5c1d" />


Author: Nguyễn Thị Ánh Minh

Date: 2025/04/20

Tools Used: POWER BI

---
# 📑 Table of Contents


--- 
# 📌 Background & Overview

## Objective 

**📖 What is this project about?**

This project centers around **analyzing global sales data from Superstore**, a retail company operating across multiple countries and regions. The vital objective is to **provide Senior Management** with important insights related to strategic decisions and market expansion. 

**What Business Question will it solve?**

- Monitor the company's overall **business performance** across regions and product categories

- Identify **key markets for potential expansion** based on sales growth and profitability.

- Determine which products are performing well and which may need to be reconsidered

  By addressing these business needs, the dashboard provides a strategic decision-making tool that enables stakeholders to make data-driven choices on market penetration and product investment.

  **👤 Who is this project for?**

  - Senior Management
 
  - Regional Sales Directors
 
  -  Product Managers
 
  -  R&D Directors
 
  -  Business Analysts and Data Analysts
 
---
# 📂 Dataset Description & Data Structure 

- Source: SuperStore sample dataset

- Format: `.csv` files

- Table: Comprises 3 main tables, including  `Orders`(Transaction details), `People` (Regional personnel information), and `Returns` (Returned transactions)
  
    - `Orders` & `Returns`: Fact table
 
    - `People` : Dim table

 - Data Modelling
   
   <img width="671" alt="image" src="https://github.com/user-attachments/assets/fb7d58c0-b599-4f45-957f-654b6350aa75" />

  ---
  # 🧠 Design Thinking Process

  This project leveraged Design Thinking methodology to deeply explore stakeholder goals and clearly define the dashboard's direction, ensuring it supports informed and strategic decision-making.

  ## 🔎 Stage 1: Empathize

  The first step in the Design Thinking Process, **Empathize**, focuses on gaining a deep understanding of stakeholder challenges and expectations in order to develop relevant effective solutions. 

#### 5W1H 
<img width="1013" alt="image" src="https://github.com/user-attachments/assets/d2e7f307-5631-4d3b-99f3-4bc64149cc77" />

**Summary**

- **Who?** Senior managers and directors (Sales, R&D, Product, Region).

- **What?** A dashboard providing an overview of global sales to support strategic decisions.

-**When & Where?** Used regularly in meetings and reports at the office.

- **Why**? To identify market opportunities, optimize product strategy, and drive business growth.

- **How?** By using data insights to decide on market expansion, product focus, and performance improvement.

#### Empathy Map 

<img width="589" alt="image" src="https://github.com/user-attachments/assets/7fcffdd0-b672-4486-8e78-11b7251de21f" />

**Summary**

- **Thinking & Feeling:** Stakeholders are concerned about identifying the right markets and products for expansion, fearing high costs of wrong decisions.

- **Seeing:** They are overwhelmed by fragmented, unstructured data and constantly changing market dynamics.

- **Saying & Doing:** They express urgency in understanding performance and competition, and often engage in cross-functional meetings to make strategic decisions.

- **Pains:**

  - Time-consuming data gathering from multiple sources

  - Inconsistent data quality

  - Difficulty identifying high-potential markets and root causes of high return rates

- **Gains:**

  - A clear, insightful dashboard to instantly grasp business performance

  - A tool to support market expansion and strategic product selection

  - Ability to forecast market trends for long-term planning

- **Stakeholder Needs – Key Questions**

  - Which markets are suitable for expansion?
  
  - What are the best-performing or strategic products?
  
  - How can we maximize revenue and growth?
  
  - How to detect and resolve issues early?
  
  - How to ensure decisions are data-driven and compelling?

#### Data Set 

<img width="268" alt="image" src="https://github.com/user-attachments/assets/abbfa6aa-132f-46e8-8ff7-cda67ab5ad55" />

## ✍️ Stage 2: Define


---
# 🌈Main Process: 

## 1. DATA PREPARATION (POWER QUERY & DAX) 

- Created relationships between 3 tables through primary keys within POWER BI

- Performed data cleaning and transformation using Power Query Editor, including handling missing values and changing data types.

- Used DAX measures and calculated columns to derive critical business metrics such as `Average Date Shipment`, `Product Profitability`.

## 2. Key insights & Visualizations 

### PAGE 1: SUPERSTORE SALES ANALYSIS OVERVIEW

![image](https://github.com/user-attachments/assets/a54f9463-4d9f-4237-967e-e97c9a54c857)

This dashboard provides a comprehensive overview of Superstore's sales performance from 2011 to 2014. 

**🧩 Key Metrics**

- **Total Revenue:** $12.64M

- **Total Profit:** $1.47M

- **Profit Margin:** 11.61%

- **Total Quantity Sold:** 178K units

- **Total Customers:** 2K

- **Return Rate:** 2.29%

**📈 Trends Over Time**

- **Revenue** and **Profit** both showed strong year-over-year growth, with revenue increasing from $2.26M in 2011 to $4.30M in 2014.

- Profit followed a similar growth pattern, indicating healthy financial performance and scalability over time.

**🌍 Regional Insights**

- The **Central region leads in total revenue ($2.82M)**, but North Asia boasts the highest profit margin (19.52%).

- **South** and **Central Asia** regions have significant room for margin improvement, indicating potential operational inefficiencies.

- Average shipping times are relatively consistent across regions (~4 days), with no clear bottlenecks.

**🌐 Market Distribution**

- The map visualization highlights high-performing markets like **Europe and North America**, where business volume and customer base are concentrated.

- This geographic data helps identify strategic regions for expansion and investment
