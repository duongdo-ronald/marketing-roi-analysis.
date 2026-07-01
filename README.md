Marketing Campaign ROI Analysis
Project Objective
To optimize marketing budget allocation and maximize profitability by analyzing the Return on Investment (ROI) across various marketing channels.

Tools Used
Data Analysis: Google BigQuery (SQL)

Data Visualization: Looker Studio

Key Insights
The [Insert Channel Name] channel delivered the highest ROI, making it the most efficient marketing lever for this dataset.

Add a brief observation here. (e.g., "Channels with lower acquisition costs did not necessarily correlate with higher conversion rates, suggesting a need for quality-focused targeting.")

[Insert your Looker Studio dashboard screenshot here]

SQL Query
This project utilized the following SQL logic to aggregate and calculate average ROI by channel:

SQL
SELECT 
    Channel_Used, 
    ROUND(AVG(ROI), 2) AS Avg_ROI, 
    COUNT(*) AS Number_of_Campaigns
FROM `marketing-roi-analysis.marketing_roi_data.data`
GROUP BY Channel_Used
ORDER BY Avg_ROI DESC;
