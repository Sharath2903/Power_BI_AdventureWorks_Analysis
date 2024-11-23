# AdventureWorks - Bike Store Sales Analysis with Power BI (Personal Project)

## Overview
Adventure Works is a bike manufacturer and seller and in this project I analyze their sales and returns data using Microsoft Power BI Desktop. This was an end to end project beginning with importing and data cleaning and ending with the creation of visuals and optimization of those visuals.

## Data Cleaning
The raw data set came in .csv format and was imported to Power BI directly. A total of 8 files were imported, each being their own table. Here I was able to get a general overview of the data set and saw that I would primarily be working with Sales and Returns data. I then began cleaning the data by ensuring columns were titled appropriately, they were in their correct data types, looking for missing data (which there was none) and began looking for what relationships I might be able to create between these tables.

## Data Modeling
After ensuring my data’s accuracy and consistency, I began the process of creating a data model for my tables. I first established my data tables which are ‘Sales Data’ and ‘Returns Data’ then set work creating relationships between tables. For this project I did not find it necessary to use any relationships other than one to many. A picture of the completed model is provided for greater understanding.

![Data Model](https://github.com/Sharath2903/Power_BI_AdventureWorks_Analysis/blob/main/data_model.PNG)

## DAX Functions
**Now that I had established my table relationships, I could begin utilizing some DAX functions to analyze the data set. I started by creating basic KPI’s such as Revenue, Profit, and Total Orders which would help me to calculate more advanced metrics later on. Some of the DAX functions I used the most include:**

**ITERATOR FUNCTIONS (SUMX):** These are formulas which evaluate an expression based on each row and then aggregate the results.
- CALCULATE(): acts as an overriding filter to give you a new filter context. Was incredibly useful for establishing Previous Months Orders, Revenue, Profit, 
  Returns and Overall Average Price
- RELATED(): This function allows you to pull data from different tables as long as there is an established many to one relationship.
- Date Functions(DateAdd, DATESINPERIOD): These date functions were very helpful when establishing a 90 Day Rolling Profit as well as the Previous Months Order, 
  Profit, Revenue and Returns.
- The measures which were created for this project were placed into their own specific Measure Table.

## Data Visualization
A total of 3 visualization pages were created for this report, these include:

**1. Sales Dashboard** 
Home to company wide KPI’s, Trending Revenue, Orders as well as several lists of the top selling products.

![Sales Dashboard](https://github.com/Sharath2903/Power_BI_AdventureWorks_Analysis/blob/main/sales_perfomance.PNG)

**Key Takeaways**
- AdventureWorks achieved $24.9M in revenue, $10.5M in profit, and processed 25.2K orders with a 2.2% return rate. 
- Revenue trends show consistent growth, peaking at $1.83M in January 2022, with Accessories leading in orders (17.0K).
- Top products include the Water Bottle and Mountain Tire Tube, while Sport-100 Helmets have higher return rates (3.3%). 
- Tires and Tubes are the most popular product type, both in sales and returns.
- Strong growth trends are evident, particularly in the Accessories category.
- Products with high return rates (e.g., Sport-100 helmets) should be investigated for potential quality improvements.

**Recommendations:**
- Focus on maintaining the growth momentum in Accessories and Bikes.
- Investigate the reasons behind higher return rates for helmets.
- Leverage the popularity of tires and tubes with targeted marketing campaigns.
- This concludes the performance analysis for AdventureWorks. Further exploration into customer feedback and competitive benchmarks could provide deeper insights into sustaining growth and minimizing returns.

**2. Regional Sales Performance Report**

This report provides a geographic overview of sales performance across key regions: Europe, North America, and the Pacific. It highlights country-level contributions and provides insights into regional segmentation using a map-based visualization.

![map_dashboard](https://github.com/Sharath2903/Power_BI_AdventureWorks_Analysis/blob/main/Map_dashboard.PNG)
**Key Takeaways:**
- North America demonstrates the highest contribution overall, particularly led by the United States.
- Europe shows consistent performance with multiple countries contributing evenly.
- The Pacific region, though represented solely by Australia, shows a notable contribution.

**Recommendations:**
- Expand in North America: Focus on strengthening operations and marketing in the U.S. while exploring growth opportunities in Canada.
- Leverage European Diversity: Utilize balanced contributions from key countries like the U.K., France, and Germany to drive regional growth through localized 
  strategies.
- Grow in the Pacific: Investigate additional market opportunities to complement Australia's strong performance in the region.

**3. Customer Insights**

  This dashboard provides an insightful overview of customer performance metrics, focusing on unique customers, revenue per customer, and customer segmentation 
  based on income and occupation. Below is a detailed analysis:

![customer_detail](https://github.com/Sharath2903/Power_BI_AdventureWorks_Analysis/blob/main/customer_dashboard.PNG)

**Key Takeaways:**

- The business engaged 17.4K unique customers, generating a Average revenue per customer of $1.431K over the period (2020–2022).
- Revenue per customer experienced a decline from early 2020, with recovery trends visible in 2022.
- Customers in the high-income group accounted for nearly 47% of total orders, demonstrating significant purchasing power.
- Occupation data shows 43.41% of total orders coming from a dominant group, making them a key demographic for targeted marketing efforts.

**Recommendations:**

- Strengthen High-Income Segment: Prioritize marketing and premium offerings for high-income customers to maximize revenue potential.
- Boost Top Customers’ Engagement: Introduce loyalty programs or exclusive benefits for high-order customers to reinforce retention and drive repeat business.
- Address Revenue Decline: Investigate causes of the revenue drop between mid-2020 and 2021 and implement strategies like promotions or product innovations to 
  sustain growth.
- Leverage Occupation-Based Data: Design occupation-specific campaigns targeting the largest demographic to increase engagement and sales.
  Monitor Revenue Recovery: Continue tracking revenue per customer to ensure sustained improvement and adjust strategies as needed.

##Conclusion##
Analyzing customer behavior, geographic trends, and sales performance through an integrated lens highlights the interconnected dynamics of business operations. The data reveals not only overall revenue patterns but also how customer demographics and regional factors influence outcomes. For those interested in leveraging data-driven strategies, such analyses provide valuable insights into optimizing performance and shaping future business growth.










