# supply-chain-logistics-dashboard
Interactive Excel dashboard created to analyze fulfillment speeds, carrier reliability, and regional shipping costs.

# Project Overview
This project is about analyzing shipping performance, carrier reliability, and delivery costs. I built an interactive dashboard to help the logistics team identify where delays are happening, which carriers are underperforming, and how freight expenses are split across regions.

# Tools Used
- Microsoft Excel

- Power Query (for data cleaning and combining tables)
    
- Pivot Tables & Charts (for data analysis and building the dashboard)

# Dataset

- The data came from two different sources/sheets:

- Orders: Contains order IDs, customer segments (Corporate, Retail, E-commerce), regional zones, and order dates.
  
- Logistics: Contains shipping costs, delivery dates, and the carriers used (FedEx, DHL, BlueDart).
  

 # What I Did (Step-by-Step)
 - Merged Tables: Instead of using messy VLOOKUP formulas, I used Merge Queries in Power Query to join the Orders and Logistics tables together using a Left          Outer Join on the OrderID column.
    
 - Data Cleaning: Cleaned up missing values, fixed data types (making sure costs are currency and dates are proper dates), and calculated total transit days.
    
 - Added Logic: Created a conditional column to automatically flag rows as "On time" or "Late" based on transit targets.
    
 - Built the Analysis: Set up Pivot Tables to calculate baseline numbers like our 53% on-time rate and the 3.7-day average delivery speed.
    
 - Created Visuals: Built a dashboard page with dynamic KPI cards linked directly to pivot tables. For the regional analysis, I used a combo chart with a             secondary axis so I could show total shipping costs (columns) and average delivery days (line) together without ruining the scale.
    
 - Added Filters: Connected slicers for transit days and order IDs, along with a native timeline filter, so users can slice and dice the whole dashboard              dynamically.

   # Business Questions Answered
  - What is our overall on-time delivery rate and average shipping time?
    
  - Which shipping carriers cause the most delays? (e.g., BlueDart causing over 44% of late deliveries).
    
  - Which zones spend the most on shipping compared to how fast they deliver?
    
  - Which customer segments are facing the highest risk of late shipments?
   
   # Dashboard Elements
  - Key Metrics: Summary cards showing the 3.7-day average cycle time and the On-Time vs. Late percentage split.
      
  - Carrier Performance: Charts showing the total number of late shipments per carrier.
      
  - Regional Cost vs. Speed: A combo chart breaking down shipping costs against average transit days by zone.
      
  - Interactive Controls: Slicers and timelines linked to all charts so the data updates instantly when clicked.
    
    


