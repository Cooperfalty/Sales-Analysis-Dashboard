# Sales-Analysis-Dashboard- Dashboard using public Superstore Sales data.

**FOR EASIER READABILITY-PLEASE SEE (Store Sales Analysis.pdf) IN FILES FOR POWERPOINT VERSION.**

The objective of this project is to deliver a clear, actionable understanding of sales and profit performance across product categories and regions. By leveraging Power BI dashboards with interactive visualizations that reveal trends, highlight strengths and weaknesses, and support strategic recommendations, the analysis was designed to answer key business questions:
Which categories and regions drive the most value?
Where are profit margins lagging?
How do discounts and customer segments impact profitability?
What actions can maximize future growth and efficiency?

MY PROCESS

1. Dataset Selection & Initial Assessment
I began by sourcing a publicly available dataset—Sample Superstore.csv—because it contains a rich mix of fields suitable for advanced analytics, including order dates, product hierarchies, sales, profit, discounts, and regional attributes. The dataset’s 10,000+ rows also made it ideal for demonstrating performance handling, data shaping, and modeling in Power BI. Before importing, I reviewed the data structure to understand relationships, potential issues, and opportunities for calculated metrics.

2. Data Cleaning & Transformation

After importing the dataset into Power Query, I performed a full data preparation:
- Data Type Enforcement: Ensured all fields were assigned correct data types (date, whole number, decimal, text, percentage) to prevent calculation errors in DAX.
- New Columns Created in Power Query:
  - Profit Margin = Profit / Sales
  - Average Order Value = Sales / Quantity
- Data Quality Steps:
  - Removed duplicates and blank rows.
  - Checked for outliers in discount and sales fields.
  - Split and merged columns where needed for cleaner hierarchies.
  - Normalization: Renamed fields, standardized category values, and applied consistent formatting.

This ensured a clean, optimized dataset.

3. Data Modeling & DAX Measures

Once loaded, I structured the dataset into a proper star-schema data model, including defining hierarchies (Category > Sub-Category) and creating a dedicated Date Table using DAX (marked as a Date Table for time intelligence accuracy).

Next, I built a library of DAX measures to support deeper business insights:

- Sales & Profit Metrics
  - Total Sales
  - Total Profit 
  - Profit Margin %
- Time Intelligence Measures
  - YOY Sales %
  - YOY Profit Change
  - 3-Month Moving Average
- Cumulative Metrics
  - Cumulative Sales
  - Cumulative Sales %
    
These DAX measures allowed me to unlock advanced insights such as trend detection, performance comparisons, forecasting behaviors, and contribution analysis.

4. Dashboard Development & Insight Storytelling

Finally, I created four separate dashboards to showcase region performance, category performance, discount impact on profit, and YOY trends analysis to then tell a story of each based on the data. All dashboards include interactive slicers and cross-filtering, enabling users to drill into region, category, year, or customer segment for more granular analysis. I also optimized the layout for usability by implementing consistent color themes, bookmarks, and navigation buttons.


**FIRST DASHBOARD: OVERVIEW EXECUTIVE SALES AND PROFIT SUMMARY**
<img width="2075" height="1139" alt="image" src="https://github.com/user-attachments/assets/30050e15-b1b1-4247-856d-25095952ee23" />
I created the overview dashboard to give a high-level view over the entire business showing total sales, profit, top products and regions, and trends through the past years for all available data. 
Insights on this overview inform me of what I may want to dig deeper into my segmented dashboards for specific recommendations. 

1. Technology leads in sales across all regions, while also producing the highest profit and margin overall.
  
2. Furniture profits and margins are lowest across all regions.
  
3. Central region has 3rd highest sales yet lowest profit and a negative 10% margin. 


**SECOND DASHBOARD: REGIONAL SALES AND PROFITABILTY**
<img width="2075" height="1162" alt="image" src="https://github.com/user-attachments/assets/5c95e13d-3442-4b89-8d02-d16ac31fd484" />
The regional performance dashboard shows performance by region (Obviously ). It provides how the business is performing in different regions based off sales and profit, unlocking insights of where and how the business is performing well or lacking. Slicer/filters were added for ability to drill down into specific categories and cities in each region to drill down deeper by region. 

1.Central region is third in sales but has the lowest profit and margin (-10.4%) while yielding the largest discount amount. Discount being highest yet profit being lowest is a red flag that promotional strategies and potential operational inefficiencies are at play in Central region. (Central KPIs Shown below) **Serious review of Central operations, discount/promotions and store strategy is needed to uncover what Central is doing differently than the other regions which leads it to be the only region with negative margin.**
<img width="750" height="100" alt="image" src="https://github.com/user-attachments/assets/8a28931c-c715-4ec9-8a92-81fd7de039cc" />

2. West Region leads in sales, profit, and profit margin. **This should prompt a review and analysis of operations, promotional strategy, and marketing in this region and standardize across the other regions since there are clearly some best practices here. To implement strategies that translate across regions, do a phased rollout by region to see which are most impactful.**
   
3.South has the lowest sales ($391,721.91) but a reasonable margin (14.54%).**I recommend launching targeted campaigns and reasonable promotions to boost volume without sacrificing much margin.**

**THIRD DASHBOARD: Category Performance and Profitablity**
<img width="2075" height="1159" alt="image" src="https://github.com/user-attachments/assets/66422430-593e-4734-885a-7f949986fb58" />
The category performance dashboard shows performance by category- furniture, technology, and office supplies. KPIs of sales, profit, and % of sales for each can provide insight on which categories do well and why. Slicers to segment by specific region, category, and customer segment being sold to are added to drill into performance as specific as you can get. The table also allows you to drill down by specific products in each category to show sales and profit for each. 

Sales by Category:                               Profit by Category: 
Technology: $836,154.03 (36.4%)                  Technology: $145,454.95 (15.61% margin)
Furniture: $741,999.80 (32.3%)                   Furniture: $18,451.27 (3.88% margin)
Office Supplies: $719,047.03 (31.3%)             Office Supplies: $122,490.80 (13.8% margin)

1.Technology has the best sales and profit/profit margin.**Increase marketing spend to further accelerate sales growth.**

2. **The second highest technology product in sales yields a -8% profit margin. After further investigation, the average discount on this product is 50%. I would recommend a reduction to a maximum 40% discount, then the profit margin would be a minimum 2% or greater depending on the discount reduction spread. =**

3. Furniture, accounts for 32% of sales (2nd highest) yet has 3.88% profit margin. **This prompts a review of the cost of goods, pricing, or promotional issues within Furniture. Target an incremental increase in profit margin by shopping for different suppliers/manufacturers, adjusting price, and reducing discounts.**

**FOURTH DASHBOARD: Discount Impact**
<img width="2076" height="1176" alt="image" src="https://github.com/user-attachments/assets/08995938-41dd-485c-ab83-1de8bb24129e" />
Discount Impact Dashboard highlights the correlation and impact discounts have on the sales and profitability of a category. Obviously, there is direct correlation with higher discounts leading to lower, and in many cases negative, profits and margins. While the higher discounts may have limited offering, it shows sales volume doesn’t increase enough to offset profit. 

1.Furniture offers the highest volume of relative sales at a 20% discount or above. Some as high as 70%.**I recommend setting a cap at 20%, as everything above is not profitable (with exception). To maintain or increase sales volumes, everyday pricing could be adjusted to eliminate the need for high discounts on select products to mitigate the negative profit margins.**

**2. Eliminating all discounts over 20% for office supplies would improve profit margin to 25% from 14%, while only sacrificing 6% of overall sales. The table shown below shows the effect  on profit, margin, and sales after eliminating all discounts over 20% for all categories on**.
<img width="1794" height="216" alt="image" src="https://github.com/user-attachments/assets/8e45e5ae-29f1-4e69-a532-65f601056485" />


FINAL DASHBOARD: Trends Analysis
<img width="1197" height="679" alt="image" src="https://github.com/user-attachments/assets/185bfe06-ffe4-423e-b73c-d25d898b6b86" />
The trends analysis shows sales and profit chronologically for the entire timeline of this data chronologically. It also shows Year over year overall sales trends for all categories, segments, and regions. However, the slicers allow you to investigate specifics for each of the named for segmented analysis. 

1. Expected CPG industry Q3 and Q4 spikes around holidays. **Inventory and demand forecasting need to account and prepare for spikes, create a demand and inventory forecasting report to reduce risk of stock outs**.

2. Sales have been steadily growing year over year. Revisit lacking categories and products to potentially cut or reposition underprfoming regions, categories, or products. Contiue to invest in the highest perfoming products, categories, and regions to gain further marketshare and increase steady growth.


