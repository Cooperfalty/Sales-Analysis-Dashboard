# Sales-Analysis-Dashboard- Dashboard using public Superstore Sales data.

The objective of this project is to deliver a clear, actionable understanding of sales and profit performance across product categories and regions. By leveraging Power BI dashboards with interactive visualizations that reveal trends, highlight strengths and weaknesses, and support strategic recommendations, the analysis was designed to answer key business questions:
Which categories and regions drive the most value?
Where are profit margins lagging?
How do discounts and customer segments impact profitability?
What actions can maximize future growth and efficiency?

MY PROCESS: 
1. First, I found a public dataset that could be suitable for this project (Sample Superstore.csv). I chose this dataset because it included order date, sales, profit, quantity, discount amount, categories, and region so I could drill down and combine different datapoints to extract insights and answer common business questions. It also included 10,000+ rows initially to show my ability to use syndicated data efficiently.
2. After downloading the dataset, I had to clean and prepare it for visualizations. I added columns- profit margin, average order value, then formatted the columns to correlate with date, numeric, text, or percentage to enable calculations.
3. Once the data was imported into Power BI, I used Dax formulas to create new calculations and data measures to unlock new insights- I added Cumulative Sales %, total profit, total sales, and 3-month moving average.
4. Finally, I created four separate dashboards to showcase region performance, category performance, discount impact on profit, and YOY trends analysis to then tell a story of each based on the data. Each dashboard allows for filtering to drill down into specific region, category, year, or segment for more microscoped analysis. 

FIRST DASHBOARD: OVERVIEW EXECUTIVE SALES AND PROFIT SUMMARY
<img width="2075" height="1139" alt="image" src="https://github.com/user-attachments/assets/30050e15-b1b1-4247-856d-25095952ee23" />
I created the overview dashboard to give a high-level view over the entire business showing total sales, profit, top products and regions, and trends through the past years for all available data. 
Insights on this overview inform me of what I may want to dig deeper into my segmented dashboards for specific recommendations. 
Technology leads in sales across all regions, while also producing the highest profit and margin overall. 
Furniture profits and margins are lowest across all regions. 
Central region has 3rd highest sales yet lowest profit and a negative 10% margin. 
<img width="3146" height="347" alt="image" src="https://github.com/user-attachments/assets/681091fb-60e0-495a-a2b4-a048c83324f3" />

SECOND DASHBOARD: REGIONAL SALES AND PROFITABILTY DASHBOARD
<img width="2075" height="1162" alt="image" src="https://github.com/user-attachments/assets/5c95e13d-3442-4b89-8d02-d16ac31fd484" />
The regional performance dashboard shows performance by region (Obviously ). It provides how the business is performing in different regions based off sales and profit, unlocking insights of where and how the business is performing well or lacking. Slicer/filters were added for ability to drill down into specific categories and cities in each region to drill down deeper by region. 
Central region is third in sales but has the lowest profit and margin (-10.4%) while yielding the largest discount amount. Discount being highest yet profit being lowest is a red flag that promotional strategies and potential operational inefficiencies are at play in Central region. (Central KPIs Shown below) **Serious review of Central operations, discount/promotions and store strategy is needed to uncover what Central is doing differently than the other regions which leads it to be the only region with negative margin.**
<img width="750" height="100" alt="image" src="https://github.com/user-attachments/assets/ca204907-2aa5-4811-bc2f-97a71183999e" />

West Region leads in sales, profit, and profit margin. **This should prompt a review and analysis of operations, promotional strategy, and marketing in this region and standardize across the other regions since there are clearly some best practices here. To implement strategies that translate across regions, do a phased rollout by region to see which are most impactful.**
South has the lowest sales ($391,721.91) but a reasonable margin (14.54%).**I recommend launching targeted campaigns and reasonable promotions to boost volume without sacrificing much margin.**
<img width="7295" height="393" alt="image" src="https://github.com/user-attachments/assets/78675427-9735-4c38-b5c8-7cf1a2f85845" />

