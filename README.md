## Sales Performance Dashboard | Power BI

### Dashboard Link : C:\Users\ACER\OneDrive\New Begining\New Begining\Projects\Project Power BI  sALES

## Problem Statement
This Sales Performance Dashboard was developed to help business stakeholders monitor and analyze overall sales performance, product performance, profitability, discounts, and customer orders. The dashboard provides interactive insights into sales trends, product-wise performance, geographical sales distribution, and period-over-period comparisons.

Using interactive filters and DAX measures, users can compare business performance across different periods, identify top and bottom performing products, analyze sales trends over time, evaluate discount strategies, and drill down into order-level details.

The dashboard enables decision-makers to:

Identify the best and worst performing products.
Analyze sales trends across different time periods.
Compare business performance between any two selected periods.
Understand the relationship between sales and profit.
Monitor discounts offered under different promotion categories.
Analyze city-wise sales performance.
Explore detailed order-level information using interactive filters.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Opened Power Query Editor and verified data quality using: 
Column Quality, Column Distribution, Column Profile.
- Step 3 :Performed data cleaning and ensured appropriate data types were assigned to all columns.
- Step 4 : Created a Star Schema Data Model consisting of:
          Fact Table
          Dim Product
          Dim Customer
          Dim Promotion
          Date Table
Established relationships between all dimension and fact tables.
- Step 5 : Created a dedicated Date Table to support time intelligence calculations.
- Step 6 : Created DAX Measures including:
           Total Sales
           Total Profit
           Total Quantity Sold
           Net Sales
           Total Orders
           Average Discount
- Step 7 :Designed the Product Performance Dashboard containing:
          Top 5 Products by Sales
          Bottom 5 Products by Sales
          Top 5 Products by Profit
          Bottom 5 Products by Profit
          Top 5 Products by Quantity Sold
          Bottom 5 Products by Quantity Sold

         Interactive slicers added:
         Date
         State
         City
         Product Line
- Step 8 :Designed the Executive Sales & Period Comparison Dashboard including:
          Total Orders KPI
	  Sales Trend Analysis
          Profit vs Net Sales Scatter Chart
          Average Discount by Promotion Category
          Sales Comparison between two selected periods
          Profit Comparison between two selected periods
          Quantity Comparison between two selected periods
          Sales by City
- Step 9 : Designed the Order Details Dashboard containing an interactive table displaying:
           Order ID
           Customer ID
           Product ID
           Product Name
           Sales
           Profit
           Discount
           Discount Percentage
           Net Sales
           Quantity Sold
           Promotion
           Order Date

          Interactive slicers added:
          Date
          Customer
          Product
          Promotion Category
- Step 10 : Applied a consistent dashboard theme, formatted KPI cards, charts, and slicers, and optimized the report layout for improved user experience.
- Step 11 : Published the report to Power BI Service.
# Product Performance Dashboard

![Product Performance Dashboard](https://github.com/user-attachments/assets/a20aaee4-9ad8-41c7-8519-23acaa5a0ca4)


# Executive Sales & Period Comparison Dashboard
![Executive Dashboard](https://github.com/user-attachments/assets/83128597-1554-43ff-a066-2daf92849c38)

# Order Details Dashboard

![Order Details Dashboard](https://github.com/user-attachments/assets/0743ea36-330e-48d2-b5f2-2af02b639bca)





- DAX Measures Used

  Examples of key measures created:

  Total Sales = SUM('Fact Table'[Total Sales])

  Total Profit = SUM('Fact Table'[Profit])

  Total Quantity Sold = SUM('Fact Table'[Units Sold])

  Total Orders = DISTINCTCOUNT('Fact Table'[Order ID])

  Average Discount = AVERAGE('Fact Table'[Discount])



- Insights

   Product Performance

  - Identified the Top 5 and Bottom 5 products based on Sales.

   - Identified the Top 5 and Bottom 5 products based on Profit.

  - Identified the Top 5 and Bottom 5 products based on Quantity Sold.
       

-  Sales Trend Analysis
  
    Analyzed sales trends over daily, monthly, quarterly, and yearly periods.
    
    Enabled drill-down analysis using the Date hierarchy. 

![Sales Trend Analysis](https://github.com/user-attachments/assets/a4374c9d-2ba5-4cc8-89ee-3c919044d928)

 
 
 - Sales vs Profit

   Scatter chart visualized the relationship between Net Sales and Profit.

   Helped identify highly profitable products and potential outlier

![Sales vs Profit](https://github.com/user-attachments/assets/320bdf87-8957-4814-9ec7-0610d62ec0c7)
 
- Period Comparison
   Users can compare any two selected periods to analyze changes in:
   Sales
   Profit
   Quantity Sold



- Discount Analysis

  Average discount offered under each Promotion Category was analyzed to understand promotional effectiveness.
  This allows quick evaluation of business performance over time.


- Order Analysis

   Interactive order-level reporting allows filtering using:
   - Product
   - Customer
   - Promotion
   - Date
   - Users can explore complete transaction details for better   business insights

 - Tools & Technologies Used
   - Power BI Desktop
    - Power Query
    - DAX
    - Data Modeling
    - Star Schema
    - Microsoft Excel

- Skills Demonstrated
   - Data Cleaning
    - Data Transformation
     - Data Modeling
    - DAX Measures
    - Time Intelligence
     - Interactive Dashboard Design
     - Business Intelligence
    - KPI Development
    - Data Visualization
    - Report Publishing

- Future Improvements
   - Add forecasting using Power BI Analytics.
   - Implement Row-Level Security (RLS).
   - Connect the dashboard to a live SQL database.
    - Schedule automatic dataset refresh using Power BI Service.
