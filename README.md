                                   ***SQL JOINs and Window Functions Project***





**1.Business Problem** 



This project analyses sales data for a retail company. The objectives is to understand customer behaviour,

product performance, and sales trends across different periods. SQL JOINs and Window Functions are used to extract meaningful business insights for decision-making



**2.Business Context**

 

The company operates in the retail industry and manages customer purchases across multiple products.

The sales department needs analytical reports to evaluate performance and improve marketing strategies.





**3.Data Challenge** 

 

  The challenge is to combine data from multiple related tables and perform advanced analytical queries.

  Simple aggregation is not sufficient; window functions are required to analyze trends and rankings.



**4.Expected Outcome**



The expected outcome is to identify top-performing products, segment customers based on spending,

and analyze sales evolution over time to support business decisions.



**5.Database Schema** 



The database schema consists of three main tables: Customer, Product, and Transaction.

The Customer table stores customer information, the Product table contains product details,

and the Transaction table records sales transactions linking customers and products.

Primary and foreign keys are used to maintain data integrity.



**6.Part A-SQL JOINs**



 **--Part A: SQL JOINs**

     

   This section demonstrates the use of different SQL JOIN types to analyze relationships

    between customers, products, and transactions.



**--INNER JOIN (screenshot P1--1)**



    The INNER JOIN retrieves transactions that have valid customers and valid products.

    This helps analyze completed sales records where all relational data is present.



**--LEFT JOIN (screenshot P1--2)**



    The LEFT JOIN is used to identify customers who have never made any transaction.

    This insight is useful for targeting inactive customers.



**--RIGHT JOIN (screenshot P1--3)**



    The RIGHT JOIN (or FULL OUTER JOIN) identifies products that have no associated sales.

    This allows the business to detect underperforming or inactive products.



**--FULL OUTER JOIN (screenshot P1--4)**



   The FULL OUTER JOIN compares customers and products, including records without matches.

   It provides a complete view of all entities regardless of activity.



**--SELF JOIN (screenshot P1--5)**



  The SELF JOIN compares customers within the same region or transactions within the same period.

  This helps identify patterns or similarities among related records.



**7.Part B-Window Functions** 



**--Ranking Functions (screenshot P1--6)**



   ROW\_NUMBER(), RANK(), DENSE\_RANK(), PERCENT\_RANK() are used to rank customers or products

   based on revenue or sales performance. These functions allow us to identify the top N entities

   and compare their relative positions.

 

**--Aggregate Window Functions (screenshot P1--7)**



    SUM(), AVG(), MIN(), MAX() with OVER() clauses are used to calculate running totals,

    moving averages, and trends over specified partitions and ranges. These functions help

    to analyze cumulative sales, average revenue, and other aggregate metrics across periods.



   

**--Navigation Functions (screenshot P1--8)**

  

   LAG() and LEAD() functions are used to compare values between consecutive rows

   within a partition. These functions allow period-to-period comparisons and

   calculation of growth or differences between sales periods.

     

**--Distribution Functions (screenshot P1--9)**



   NTILE(4) and CUME\_DIST() are used for customer segmentation and distribution analysis.

   They help to categorize customers into quartiles or calculate their cumulative distribution

   for marketing or analytical purposes.



  

   

**8.Results Analysis** 



--- Descriptive: The queries show the top products, customer rankings, and sales trends.

--- Diagnostic: These results help understand why certain products are performing well

                and which customers are more active or inactive.

--- Prescriptive: Based on the analysis, targeted marketing can be applied to top customers,

                 and inventory or promotions can be adjusted for products with low sales.





**9.References** 

  

   - Oracle Official Documentation: https://docs.oracle.com

   - SQL Tutorials: https://www.w3schools.com/sql/

   - Academic resources used during the course ⁠



**10.Integrity Statement** 



   All sources were properly cited. Implementations and analysis represent original work.

   No AI-generated content was copied without attribution or adaptation.

                       ***Final Checklist***

          - [x] PDB created successfully
          - [x] User created inside the PDB
          - [x] Temporary PDB created and dropped
          - [x] OEM dashboard accessed
          - [x] Screeshots uploaded
          - [x] Repository is Public 
          

          

    




