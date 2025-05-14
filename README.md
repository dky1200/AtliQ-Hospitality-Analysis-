# AtliQ-Hospitality-Analysis-
Domain: Hospitality | Tech Stack: Power BI, SQL, Data Analysis

Live Dashboard Link : https://app.powerbi.com/groups/b388d402-015c-4b08-8178-6124bc45fd10/reports/7ed6f96c-23d1-4602-b06d-1eb02afc767b?ctid=c6e549b3-5f45-4032-aae9-d4244dc5b2c4&pbi_source=linkShare&bookmarkGuid=9b11d2eb-04e6-4434-b0a7-cdea8bcb6430

![image](https://github.com/user-attachments/assets/c53474f0-8049-46c1-a712-4c7aa198a38c)

AtliQ Hardware, a leading computer hardware manufacturer, needed clear visibility into its regional sales performance. To solve this, I built a comprehensive Sales Data Analysis Dashboard using 𝗦𝗤𝗟, 𝗗𝗔𝗫, and 𝗣𝗼𝘄𝗲𝗿 𝗕𝗜, unlocking actionable insights to help drive data-backed decisions. Here’s a breakdown of how it helped:

🔍 𝙆𝙚𝙮 𝘾𝙝𝙖𝙡𝙡𝙚𝙣𝙜𝙚𝙨:
Regional Disparities: Delhi NCR dominated revenue (52.8%), while Bengaluru faced a -20.8% profit margin.

Profitability Gaps: Some markets had strong revenues but lagged in profit margins.

Zonal Insights: The North Zone contributed 68.6% of revenue, but the Central Zone led in profitability (42.23%).

Project Overview
A data-driven analysis of 3 months of hotel booking data to identify revenue leakage, occupancy trends, and pricing inefficiencies for AtliQ Grands (a luxury hotel chain). Developed a Power BI dashboard to visualize KPIs and actionable insights, enabling the revenue management team to:

Recover ₹251.1M in potential revenue.

Increase realization rate from 70.14% to 80%.

Optimize dynamic pricing and cancellation policies.


Key Metrics

 ![image](https://github.com/user-attachments/assets/eb797eec-cf05-4b7f-9c23-267e01d96976)

 Insights & Solutions
1. Revenue Leakage
Problem: 30% revenue loss (24.84% cancellations + 5.02% no-shows).

Solution:

Implement tiered cancellation fees (e.g., 50% refund if canceled >72hrs).

Introduce pre-authorization holds to reduce no-shows.

2. Low Occupancy Weeks
Problem: Weeks W21, W23, W26, W30, W31 underperformed.

Solution:

Dynamic pricing: Lower rates for these weeks.

Promotions: "Weekday Staycation" packages.

3. Booking Channel Optimization
Top Channel: MakeYourTrip (20.02% bookings).

Action: Negotiate lower OTA commissions + boost direct bookings via loyalty programs.

4. Room-Class Performance
![image](https://github.com/user-attachments/assets/e476d256-3820-450f-930d-9f083640393a)


Dashboard Features
Interactive Filters: City, room class, date range.

Visualizations:

Heatmaps (occupancy trends).

DBRN vs. DURN gap analysis.

Revenue by city/room class.

Alerts: Highlight low-realization weeks.

Technical Details
Data Sources: SQL database (booking records, cancellations).

Transformations: Cleansed null values, added calculated columns (e.g., realization rate).

Measures: DAX for WoW comparisons (e.g., RevPAR WoW%).

sql
-- Sample Query (Revenue by City)
SELECT city, SUM(revenue) AS total_revenue 
FROM bookings 
GROUP BY city 
ORDER BY total_revenue DESC;
How to Use
Clone the repo:

bash
git clone https://github.com/dky1200/AtliQ Hospitality Analysis.git
Open in Power BI: AtliQ Hospitality Analysis.pbix.

Adjust filters: Explore data by date/city/room type.

Future Work
Predict cancellations using ML (Python + Scikit-learn).

Integrate live data feeds for real-time monitoring.

 

 
  

