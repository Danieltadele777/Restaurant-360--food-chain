### Restaurant-360

Conducting an in-depth analysis of Restaurant 360, comprising 21 stores. The analysis will encompass 3,924,748 orders spanning from 2015 to 2020. Four primary datasets will be utilized: Order Data, Orderline, Payment Data, and ID Store.
## Table of contents
 - [Project Overview](#project-overview)
 - [Data Source](#data-source)
 - [Tools Used](#tools-used)
 - [Data cleaning](#data-cleaning)
 - [Exploratory data analysis](#exploratory-data-analysis)
 - [Hypothesis Testing](#hypothesis-testing)
 - [Data Analysis](#data-analysis)
 - [Findings](#findings)
 - [Recommendations](#recommendations)
 - [Limitations](#limitations)
 - [References](#references)

### [Project Overview]()

The aim of this analysis is to extract valuable insights and trends regarding customer behavior, sales performance, and store operations over the specified timeframe.

[CLICK ME to access presnetation video and Power BI dashboards](https://github.com/Danieltadele777/Restaurant-360-Video-presentation-and-dashboards.git)

<img width="1239" alt="Global" src="https://github.com/Danieltadele777/Restaurant-360--food-chain/assets/147874875/5bfd2652-d897-4a8f-9816-9ef9f20b511d">



### [Data Source]()

The data source used for this analysis is provided by the bootcamp provider. The school also provided detailed information about join keys and data schemas. 

### [Tools Used]()
- Google BigQuery: Primary data cleaning
- SQL: For data claning and transformation
- Panda: For data cleaning, inspection and analysis
- Power BI: Visualization

### [Data cleaning]()
To clean the data we performed the following tasks:
- Reading the SCHEMA, data dictionary and understanding of the Details of the data
- Handling null values and understanding the columns
- Handling missing values and duplicates
- Data cleaning, formatting and also dates and numbers adjustment

### [Exploratory Data analysis]()
- What is the overall sales trend?
- Which products are top sellers?
- What are the peak sales periods?
- Which products sold in high quantity?
- Which seller sold the most?
- Which products received low reviews?
- Which products received high reviews?
- Which products generated the highest revenue?
- What is the seasonality of orders?

### [Hypothesis Testing]()
- The number of sales higher in weekends than during the weekday
- More number of tables in the store means bigger turnover
- Bigger the restaurant (number of tables) better the time efficiency
- Average price is higher in stores closest to the city center
- More number of orders means higher turnover
- Store with more time efficiency sell more
- When higher the average price in the store bigger the turnover

### [Data Analysis]()
 - [Click here to see the SQL codes]()
 - [Click here to see the Python codes]()

Some of SQL codes used:
```SELECT
    CASE
        WHEN date_opened BETWEEN "2015-01-01" AND "2015-12-31" THEN "2015-01-01"
        WHEN date_opened BETWEEN "2016-01-01" AND "2016-12-31" THEN "2016-01-01"
        WHEN date_opened BETWEEN "2017-01-01" AND "2017-12-31" THEN "2017-01-01"
        WHEN date_opened BETWEEN "2018-01-01" AND "2018-12-31" THEN "2018-01-01"
        WHEN date_opened BETWEEN "2019-01-01" AND "2019-12-31" THEN "2019-01-01"
        WHEN date_opened BETWEEN "2020-01-01" AND "2020-12-31" THEN "2020-01-01"
        ELSE "2020-01-01"
    END AS date_corrected,
    SUM(m_cached_payed) AS total_payed,
    SUM(customer) AS total_customers,
    ROUND(SUM(m_cached_payed) / NULLIF(SUM(customer), 0), 2) AS ticket_medium
FROM `avid-infinity-402410.Tiller_by_sumup.JOIN_payment_orderdata`
GROUP BY date_corrected
```



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

### [Limitations]()

- We had to remove all null and duplicated values from the columns because they would have affected the accuracy of our analysis 
- In addition to that, we faced ambigious coloumn so we used our assumption to analyse the coloumn. Because of the limitations of the data provided, We weren't able to take further steps

### [References]()
1. [Stack Overflow](www.stackoverflow.com)
