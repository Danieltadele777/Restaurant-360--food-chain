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
<img width="1241" alt="Screenshot 2025-01-06 at 23 28 14" src="https://github.com/user-attachments/assets/345832c6-4476-4f7d-881e-980f06b6c7fd" />
<img width="1242" alt="Screenshot 2025-01-06 at 23 29 24" src="https://github.com/user-attachments/assets/75788bd7-543b-4a29-98e2-f09db4d4e746" />
<img width="1243" alt="Screenshot 2025-01-06 at 23 29 50" src="https://github.com/user-attachments/assets/97a8c764-1eeb-4c7e-9fc6-ecb3bd0fac37" />
<img width="1245" alt="Screenshot 2025-01-06 at 23 30 21" src="https://github.com/user-attachments/assets/2b019466-7350-4306-8664-0a16cbfa5933" />
<img width="1243" alt="Screenshot 2025-01-06 at 23 31 05" src="https://github.com/user-attachments/assets/5de341a7-636f-4ce5-88c8-b35a9677e935" />
<img width="1242" alt="Screenshot 2025-01-06 at 23 31 29" src="https://github.com/user-attachments/assets/5186d6c6-8b39-4e00-911d-6be9a4019f9a" />



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
