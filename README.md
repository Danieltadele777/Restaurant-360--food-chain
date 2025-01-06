### Online Restaurant Chain Analysis

Conducted an in-depth analysis of an online restaurant chain, comprising 21 stores all over Paris. The analysis will encompass 3,924,748 orders spanning from 2015 to 2020. Four primary datasets will be utilized: Order Data, Orderline, Payment Data, and ID Store.
## Table of contents
 - [Project Overview](#project-overview)
 - [Power BI dashboard](#power-bi-dashboard)
 - [Tools Used](#tools-used)
 - [Data cleaning](#data-cleaning)
 - [Exploratory data analysis](#exploratory-data-analysis)
 - [Hypothesis Testing](#hypothesis-testing)
 - [Findings](#findings)
 - [Recommendations](#recommendations)


### [Project Overview]()

The aim of this analysis is to extract valuable insights and trends regarding customer behavior, sales performance, and store operations over the specified timeframe.

### [Power BI dashboard]()

<img width="1239" alt="Global" src="https://github.com/Danieltadele777/Restaurant-360-Video-presentation-and-dashboards/assets/147874875/5991dc1a-59e0-4ab4-a2c2-b91d9be98bb6">
<img width="1236" alt="Revenue" src="https://github.com/Danieltadele777/Restaurant-360-Video-presentation-and-dashboards/assets/147874875/a174623f-3eb0-4ce5-ac13-7657c5f7f7d3">
<img width="1238" alt="category" src="https://github.com/Danieltadele777/Restaurant-360-Video-presentation-and-dashboards/assets/147874875/541c97a4-4b17-4a00-8c32-26e5f3e3f686">
<img width="1242" alt="store" src="https://github.com/Danieltadele777/Restaurant-360-Video-presentation-and-dashboards/assets/147874875/b50c1bf3-9710-467f-bfab-3d8b46e69f71">
<img width="1235" alt="item" src="https://github.com/Danieltadele777/Restaurant-360-Video-presentation-and-dashboards/assets/147874875/4daa5751-ce1c-448e-b4a8-a3b6fc071b14">
<img width="1248" alt="Paired items" src="https://github.com/Danieltadele777/Restaurant-360-Video-presentation-and-dashboards/assets/147874875/a6111915-919a-4b8e-b392-d40c57fbed8a">

### [Tools Used]()
- Google BigQuery, PostgreSQL
- SQL: For data cleaning and transformation
- Python, Panda: For data cleaning, inspection, and analysis
- Power BI: Visualization, DAX, Measures

### [Data cleaning]()
To clean the data I performed the following tasks:
- Reading the SCHEMA, data dictionary and understanding the Details of the data
- Handling null values and understanding the columns
- Handling missing values and duplicates
- Data cleaning, formatting, and also dates and numbers adjustment

### [Exploratory Data analysis]()
- What is the overall sales trend?
- Which products are top sellers?
- What are the peak sales periods?
- Which products are sold in high quantities?
- Which seller sold the most?
- Which products received low reviews?
- Which products received high reviews?
- Which products generated the highest revenue?
- What is the seasonality of orders?

### [Hypothesis Testing]()
- The number of sales is higher on weekends than during the weekday
- More number of tables in the store means bigger turnover
- The bigger the restaurant (number of tables) better the time efficiency
- Average price is higher in stores closest to the city center
- More number of orders means higher turnover
- Store with more time efficiency sell more
- When higher the average price in the store, the bigger the turnover

### [Findings]()
The analysis results are summarized as follows:

- The company sales have been steadily growing during the years 2017 and 2018, with a remarkable 230% growth rate
- During 2018 and 2019, it showed a 33% growth rate, but during 2020, the sales showed a 57% reduction
- In terms of revenue and sales, menus are the best-performing category
- Store 4151 generated €2.32 million in revenue, while other stores like 5281 and 1513 generated around €1 million in revenue each
- Orders closed on weekdays generated a higher average revenue than those closed on weekends. The average order value is approximately €56.13 for weekdays and €36.46 for weekends
- When it comes to payment method, customers tend to spend more when paying with a card compared to cash: With a card, the average payment amount is €68.92, but with cash, the average payment amount is €14.57

### [Recommendations]()
Based on the analysis we recommended the following actions:
- Always ensure that the top-selling products are in stock, especially the paired items
- Given that certain stores, such as 4151, are generating a significant amount of revenue, it may be necessary to study this store to understand the factors contributing to its performance
- It may be necessary to identify the top sellers or recognize their contributions
- Some stores sold fewer items. It may be necessary to determine the reasons and review the process
