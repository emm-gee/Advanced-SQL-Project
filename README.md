### Overview
This SQL project, developed as part of the D191 Advanced Data Analytics course, involves analyzing sales data from a DVD rental database to assess the performance of two store locations. The project leverages PostgreSQL to manage and manipulate the data.

### Components
* **Database Setup:** Utilizes the staff and payment tables from the DVD rental database to extract and analyze sales data linked to each store location.
* **Data Transformation:** Implements functions to extract month and year from payment timestamps, facilitating temporal analysis of sales data.
* **Tables Creation:** Includes the creation of sales_by_date and detailed_sales_by_date tables to store transformed data and detailed sales records, respectively.
* **Aggregation Queries:** Uses SQL queries to generate aggregated reports like total sales per store monthly and a summary table to track overall store performance.
* **Trigger and Stored Procedures:** Establishes a trigger and stored procedures for maintaining the summary table and facilitating the automatic updating of sales data.

### Functions and Procedures
* sales_by_month and sales_by_year: Functions to extract the month and year from payment dates.
* create_sales_by_date_table: A stored procedure to recreate detailed and summary sales tables as needed.
* Triggers: Set up to update the summary sales data automatically upon new data insertions.

### Automation
Integration with pgAgent for scheduling and automating the execution of stored procedures, ensuring up-to-date reporting.

### Usage
The project allows running detailed sales reports quarterly and summary tables more frequently to monitor the performance and viability of the stores over time.
