# Business-Insights-360


## Project Overview
AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.

## Power BI Project

The `.pbix` file for this project is too large for direct upload. You can download it from the following link:
[Download Power BI File from Google Drive] (https://bit.ly/4gdt696)

I worked on this project by the Codebasics PowerBi Course

## Tech Stacks

- SQL
- Power BI Desktop
- Excel
- DAX Language
- DAX Studio (for optimizing the report)
- Project Charter File


## PowerBI techniques Learnt
What are all the questions should be asked before staring the project
Creating calculated columns
creating measure using DAX language
Data modeling
Using Bookmarks to switch between two visuals
Page navigation with buttons
Using divide function to prevent zero division errors
creating date table using m language
Dynamic titles based on the applied filters
Using KPI indicators
Conditional formatting the values in visuals using icons or background color
Data validation techniques
PowerBi services
Publishing reports to PowerBi services
Setting up personal gateway to set up the auto refresh of data
PowerBi App creation
Collaboration, workspace, access permissions in PowerBi services

## GitHub
Uploading Large size files using GitHub LFS
Tracking the particular type of file extensions for LFS

## Business Related Terms

- Gross Price
- Pre-Invoice Deductions
- Post-Invoice Deductions
- Net Invoice Sale
- Gross Margin
- Net Sales
- Net Profit
- COGS - Cost of Goods Sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer


## Company’s back ground
AltiQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel

Retailers
Direct
Distributors
Recently the company has faced a unforeseen loss by opening store in America based on the surveys, intuition and some excel analysis and also the company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AltiQ hardware has no other option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry.

Project kick off session, where you should get clear of for what and why this project and all other questions you have with regards to the project

## Questions to ask before starting with dashboard
What is the objective of building this PowerBi dashboard?
In what terms the success of this project will be measured?
What will be time dead-line of the project?
do the stakeholders expecting pre-view before the actual release?
What are all the hopes stakeholders have out of this project?
what are all fears the stakeholder have in terms of building this dashboard?
Who are all will be using this dashboard and for what purpose?
what are all expectation the stakeholders have, by the completion of this project?
What can go wrong while building this project?
what are all the resources/ data needed to build this dashboard?
is there any inputs from stakeholders in terms of design and views of the dashboard?
After the project kick off meetings, the data engineering team has given the data as per the request of data analytics team, let’s explore them.

## Dataset Understanding.

Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions

- gdb041:
  - dim_customer
    - 27 distinct markets (ex India, USA, Spain)
    - 75 distinct customers throughout the market
    - 2 types of platforms:
      - Brick & Mortar - Physical/offline store
      - E-commerce - Online Store (Amazon, Flipkart)
    - Three channels:
      - Retailer
      - Direct
      - Distributors
  - dim_market
    - 27 distinct markets (ex India, USA, Spain)
    - 7 sub-zones
    - 4 regions:
      - APAC
      - EU
      - nan
      - LATAM
  - dim_product
    - Divisions:
      - P & A
        - Peripherals
        - Accessories
      - PC
        - Notebook
        - Desktop
      - N & S
        - Networking
        - Storage
    - There are 14 different categories, like Internal HDD, keyboard.
    - There are different variants available for the same product.
  - fact_forecast_monthly
    - This table is used to forecast the customer’s need in advance, which can help in:
      - Higher customer satisfaction
      - Reduced cost in warehouses for storage purposes
    - The table is denormalized by the data engineering team, as it is a data warehouse aimed for analytical work.
    - All the dates of the month will be replaced by the start date of the month.
    - It will have all the column names, and in the end, it will have the forecast quantity need of the customer.
  - fact_sales_monthly
    - This table is more or less the same as the fact_forecast_monthly table, but the last column has the value of sold quantity instead of forecast value.

- gdb056:
  - freight_cost
    - This table has details of travel costs and other costs for each market with the fiscal year.
  - gross_price
    - Has the details of gross prices with product code.
  - manufacturing_cost
    - Has the details of manufacturing costs with product code and year.
  - Pre_invoice_deductions
    - Has the details of pre-invoice deduction percentages for each customer with year.
  - Post_invoice_deductions
    - Post-invoice deductions and other deduction details.

## Importing data into PowerBi
As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential

## Data Model
-Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
-Poor data modeling affects the over all performance of the report.
-Following Good practices of data modeling is must. Refer this page to get to know the good practices Blog
-In this project, we have followed Snowfall data modeling method.

![Screenshot 2024-12-21 222411](https://github.com/user-attachments/assets/29518a70-a76e-4faf-9d68-bf9daea15f1e)


## Dashboard designing
Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required

Home view
In Home view, all the views button will be available. User will land on specific view page by clicking the button

- Info  
- Finance View  
- Sales View  
- Marketing View  
- Supply Chain View  
- Executive View  
- Products  
- Support


## Overall Report

[Uploading Screen Recording 2024-12-21 231452.mp4…](https://github.com/user-attachments/assets/df5ad827-a9c1-412f-bae9-ad5cd2ad4ccc)


## Info Page

![Screenshot 2024-12-21 220616](https://github.com/user-attachments/assets/461810bf-791a-4985-bbc9-a5e3b4722c86)

## Finance view
![Screenshot 2024-12-21 220657](https://github.com/user-attachments/assets/198fc91d-ab0c-4289-ba73-ba4f8cc25e04)

## Sales view
![Screenshot 2024-12-21 220730](https://github.com/user-attachments/assets/cfcb18c2-9993-43f8-a5e4-61b468a23144)

## Marketing view
![Screenshot 2024-12-21 220752](https://github.com/user-attachments/assets/b3e505ff-e168-4374-9747-9684fd936538)

## Supply chain view
![Screenshot 2024-12-21 220814](https://github.com/user-attachments/assets/45210876-935d-450b-9a67-e0aa6af4de28)

## Project Outcome
By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.

