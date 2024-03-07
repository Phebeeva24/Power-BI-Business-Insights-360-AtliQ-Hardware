# Business-Insights-360 [SQL | Power BI | MS Excel]
## SQL Data Exploration & Power BI Dashboard
### Domain: Financial Domain
### Project Overview:
---
AtliQ Hardware has been growing rapidly in recent years, and they have decided to implement data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data-driven decisions. This project is hoped to give answers to the questions of stakeholders in terms of all aspects like finance, sales, marketing, and supply chain.

I worked on this project by following the Codebasics PowerBi Course, The Link to the 
course is [here](https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project)



---
### Company's Background
AtliQ Hardware manufactures and sells hardware like PC, Mouse, Printers, etc to multiple companies across the world. AtliQ’s customers are companies like Croma, Amazon, Neptune, Staples, Walmart, etc.
*These customers are of two types*
- Physical Stores
- E-commerce platforms
*They sell their products through three mediums/channels,*
- Retailers
- Direct
- Distributors
### Problem Statement:
---
AtliQ Hardware is struggling to do good business in various parts of the world. So far, all the decisions that AtliQ took have been based on some surveys and intuitions.

AtliQ Team uses MS Excel for data analysis but as the business expands globally company's Top management decides to use Power BI for data analytics. So Top management wanted the analytics team to Provide insights through SQl to make decisions and as the later part of the Project, a dashboard was created for various key departments, so they can get insights on important metrics and make data-driven Decisions.
### Data Source
we used two databases. In that database, each contains some tables which are explored below.

Extracted CSV file from the database
### * gdb041
- dim_customer
- dim_product
- dim_market
- fact_sales_monthly
- fact_forecast_monthly

### * gdb056
- freight_cost
- gross_price
- manufacturing_cost
- pre_invoice_deduction
- post_invoice_deduction

### WorkFlow:
---
### MySQL WorkBench:
- Data was Loaded into Mysql and the database was designed by establishing relationships in a Snowflake schema format between the tables with ERD in MySQL.
- Data was ready for Data Analysis and key metrics were Derived, for all the requests from Product owners.
- A Data pipeline was established in deriving Metrics, with many Data Cleaning methods implemented in between.
- Stored Procedures were created for the complex Queries so that Product owners can extract reports by necessary filters.
  ### PowerBI Dashboard:
- The first step was to load the data into MySQL Database and connect it to the Power BI.
- Review and delete the Database relationship created by Power BI by default. Also, creating the required dimension table in Power Query.Data validation using some tables in Power BI and matching the values with the data provided.
- Data Transformation. For example, creating a Last Sales Month Reference table. So, the last sales month reference table will be dynamic and will change after every sale. Created calculated columns in Power Query like a fiscal year and merged the tables.
- Data modeling is a connection between different tables using a common table between them. In this project, Start Schema is used for Data Modelling where all the dimension tables were connected with Fact tables.

  ![Alt text]("C:\Users\HP\Pictures\5LINK.png")
  

 
