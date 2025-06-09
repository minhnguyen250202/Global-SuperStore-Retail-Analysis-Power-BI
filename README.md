# 📊 Global-SuperStore-Retail-Analysis-Power-BI

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

### PAGE 2: REGIONAL PERFORMANCE 

![image](https://github.com/user-attachments/assets/39964fc0-f41a-4f82-99d0-69e371304f66)

**📈 Revenue Trend by Year and Market**

- **APAC** shows steady and strong growth across the years, peaking in 2014.

- **EU** and **US** exhibit consistent upward trends, indicating expanding customer bases.

- **EMEA, Africa, and Canada** have much smaller and flatter revenue trends, indicating limited growth or market saturation.

**📉 Profit Margin by Market**

- **Canada** surprisingly leads in **profit margin (26.62%)**, likely due to high-value, low-volume transactions or effective cost control.

- Despite leading in volume, **APAC** only ranks mid-tier in margin (~11%), implying potential inefficiencies or aggressive pricing strategies.

- **LATAM and EMEA** have the lowest margins, suggesting operational challenges or high return rates in those markets.

  **📊 Total Revenue by Market and Category**

- **APAC** leads with the highest total revenue of **$3.6M**, followed by **EU **($2.9M) and US ($2.3M).

- **Canada** ranks last in revenue with just **$0.1M**, suggesting minimal market activity or late entry into the region.

**💰 Total Profit by Market**

- **APAC** also tops in profit with **$0.44M**, confirming it as the most lucrative market.

- **EU and US** follow with **$0.37M and $0.29M**, respectively.

- **Canada** again shows the weakest performance with only **$0.02M profit**, potentially due to low volume or high costs.


**💡 Key Insights**

- **APAC** is the most valuable market in both revenue and profit, making it a clear strategic focus.

- Canada, although small in size, delivers high profitability per transaction, which could be worth exploring further for niche growth.

- LATAM and EMEA markets may require operational review or marketing support to improve margins.

Regional trends support targeted strategies: invest more in APAC/EU, re-evaluate EMEA, and explore opportunities in Canada for margin-focused growth.

### PAGE 3: PRODUCT INSIGHTS 

![image](https://github.com/user-attachments/assets/26f423b2-c539-4283-9089-f1b30f44c4c6)

**1️⃣ Total Revenue by Category**

📌 Insights:

- Furniture is the top revenue-generating category.

- Technology generates the least revenue, but only slightly behind Office Supplies.

- Revenue is relatively evenly distributed, which suggests a diverse portfolio.

**2️⃣ Total Revenue by Ship Mode**

📌 Insights:

- Standard Class dominates revenue – it's the preferred shipping mode.

- Faster shipping options like First Class and Same Day contribute less, likely due to higher costs or limited availability.

**3️⃣ Total Quantity by Segment**

- Consumer segment accounts for the majority of orders (more than half).

- Corporate and Home Office segments are significantly smaller in volume.

**4️⃣ Total Profit by Category and Sub-Category**

💰 Key insights by sub-category:

- Technology sub-categories (e.g., Copiers and Phones) are the most profitable.

- Tables in Furniture show a net loss – only sub-category with negative profit.

- Other profitable sub-categories: Bookcases, Appliances, Chairs, Binders, Paper, Supplies.

- Some sub-categories (e.g., Fasteners, Labels) have very low or near-zero profit.

📌 Insights:

- Not all high-revenue sub-categories are profitable.

- Tables should be reviewed — high cost, low margin, or discounts might be affecting profitability.

- Technology is the most profitable category overall.

**5️⃣ Top 5 Highest Profit Products**

- The Canon printer is the most profitable individual product by a large margin.

- Technology products (phones and printers) dominate the profit chart.

- Furniture item (Bookcase) also makes it to the top list, showing that Furniture can still be profitable in specific SKUs.

  ### PAGE 4: GROWTH TRENDS

![image](https://github.com/user-attachments/assets/6778c615-f6c9-4674-994e-f1a1398c7ad4)


**Strong cumulative growth over the 4-year period**

- The total revenue shown represents a cumulative value from 2011 to 2014, reaching $12.6M.

- Compared to the previous 3-year period (2011–2013), there was a 51.54% increase, indicating a significant acceleration in growth in 2014.

- However, this growth should be interpreted as multi-year expansion, not a single-year leap.

**Year-over-year sales trends confirm the growth**

- The line chart shows a steady increase in monthly revenue over time, confirming consistent upward momentum.

- The spike in 2014 further supports that the last year contributed significantly to the overall growth.

**Canada stands out with the highest profit margin**

Canada consistently maintains a profit margin above 30%, significantly higher than other markets.

This suggests high pricing power or operational efficiency in that region.

**Opportunities in underperforming markets**

EMEA shows low and stagnant profit margins (~5%), which could signal issues in pricing, competition, or cost structure.

LATAM and Africa show moderate margins, but Africa displays a slight upward trend, suggesting potential for improvement.

**US and EU maintain stable but moderate margins**

Both regions show consistent profit margins around 13–14% across years.

These regions are stable but might require innovation or cost optimization to improve profitability further.

---
# 🔎 Final Conclusion & Recommendations

### 🔍 Conclusion**

The business performance of SuperStore between 2011 and 2014 reveals a strong growth trajectory. 
- Both revenue and profit have increased significantly over the years, with a peak in 2014, suggesting that the company is successfully scaling.
- Technology remains the leading category in terms of revenue and profitability, while Consumer and Corporate segments account for over 70% of sales volume.
- However, profitability varies across markets and sub-categories—Canada, for instance, shows high margins but generates relatively low revenue, and the “Tables” sub-category is the only one operating at a loss.
- Return rate has slightly decreased to 2.29%, a positive signal for operational efficiency.

Despite the overall growth, some insights suggest opportunities for strategic focus: certain regions and product lines are underperforming, while others offer high margins yet remain untapped. Aligning marketing, sales, and product strategies with these insights will allow SuperStore to optimize performance and sustain long-term growth.

### ✅ Strategic Recommendations

**1. Refine Regional Strategy**

- Focus on high-revenue markets (APAC, EU, US, LATAM) to continue scaling, while optimizing costs to maintain margins.

- Expand in Canada by boosting brand awareness, increasing ad spend, or launching localized campaigns—given its high profit margin and untapped potential.

**2. Enhance Customer Segmentation Tactics**

- Prioritize cross-sell and upsell strategies for Corporate and Consumer customers (which represent >70% of the customer base).

- Consider developing B2B-focused solutions for Office Supplies or underperforming products.

**3. Product Line Optimization**

- Double down on Technology and explore complementary upsell products (e.g., software, accessories).

- For Office Supplies, re-evaluate underperforming items or bundle offers to increase volume and profitability.

**4. Address Weak Sub-Categories**

- Investigate root causes for Tables' negative margin (pricing, shipping, returns) and pivot strategy: new pricing, bundling, or alternate sales channels.

**5. Capitalize on Hero Products**

- Leverage the success of Canon imageCLASS 2200 by increasing its visibility in campaigns and prioritizing it in supply chain and sales planning.

- Use it as a benchmark to replicate high-margin strategies for similar high-end products.

**6. Improve Data Granularity**

- Split metrics by year, not multi-year aggregates, to better track growth trends and measure performance accurately.

- This will help produce more precise YoY insights and avoid misleading growth indicators.

