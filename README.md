# SQL Data Analytics Project

## Project Overview
This project demonstrates **data exploration, analysis, and reporting** using SQL on a sales dataset.  
It includes dimension tables, a fact table, and multiple analysis scripts covering measures, rankings, trends, and customer/product reports.

---

---

## Database & Tables

### Database
- `DataWarehouseAnalytics`  

### Schema
- `gold`  

### Tables

#### 1. `dim_customers`
| Column                - Description 

| customer_key          - Primary key for customer dimension 
| customer_id           - Original customer ID 
| customer_number       - Customer unique number 
| first_name            - Customer first name 
| last_name             - Customer last name 
| country               - Customer country 
| marital_status        - Customer marital status 
| gender                - Customer gender 
| birthdate             - Date of birth 
| create_date           - Record creation date 

#### 2. `dim_products`
| Column                 - Description 

| product_key            -  Primary key for product dimension 
| product_id             -  Original product ID 
| product_number         -  Product unique number 
| product_name           - Product name 
| category_id            - Category ID 
| category               - Product category 
| subcategory            - Product subcategory 
| maintenance            - Maintenance type 
| cost                   -Product cost 
| product_line           -Product line 
| start_date             -Record start date 

#### 3. `fact_sales`
| Column                 - Description 

| order_number           - Sales order number 
| product_key            - FK to `dim_products` 
| customer_key           -FK to `dim_customers` 
| order_date             -Order date 
| shipping_date          -Shipping date 
| due_date               -Due date for delivery 
| sales_amount           - Total sales amount 
| quantity               - Quantity sold 
| price                  -Price per unit 

---

## Scripts
1. `01_database_exploration.sql` – Explore database structure and basic tables.  
2. `02_dimensions_exploration.sql` – Analyze customer and product dimensions.  
3. `03_date_range_exploration.sql` – Explore date ranges in sales data.  
4. `04_measures_exploration.sql` – Calculate key measures (sales, quantity, price).  
5. `05_magnitude_analysis.sql` – Analyze magnitude of sales.  
6. `06_ranking_analysis.sql` – Rank customers, products, or orders.  
7. `07_change_over_time_analysis.sql` – Analyze trends over time.  
8. `08_cumulative_analysis.sql` – Perform cumulative sum and metrics.  
9. `09_performance_analysis.sql` – Evaluate overall sales performance.  
10. `10_data_segmentation.sql` – Segment customers or products.  
11. `11_part_to_whole_analysis.sql` – Analyze contribution of parts to totals.  
12. `12_report_customers.sql` – Generate customer reports.  
13. `13_report_products.sql` – Generate product reports.  

---

## How to Run
1. Open **SQL Server Management Studio (SSMS)**.  
2. Create the database and schema using your scripts.  
3. Upload datasets to `datasets/csv-files/`.  
4. Run scripts in **logical order** (01 → 13) to explore, analyze, and report.  

---

## Notes
- CSV files must remain in `datasets/csv-files/` for scripts to work.  
- All tables are under schema `gold`.  
- Scripts cover **data exploration, analysis, and reporting**.  

---

## License
This project is for **learning and demonstration purposes**.

