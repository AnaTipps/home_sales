# Big-Data  Challenge Home Sales Analysis 

## Background 

In this challenge is required the use of of SparkSQL to determine key metrics about home sales data. Sparkwill be another tool will support in the creation of temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Instructions

* Import the necessary PySpark SQL functions for this assignment.

Read the `home_sales_revised.csv` data code into a Spark DataFrame.

* Create a temporary table called home_sales.

* Answer the following questions using SparkSQL:

    * What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places (`q1`).

    * What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places (`q2`).

    * What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places(`q3`).

    * What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places (`q4`).

* Cache your temporary table home_sales.

* Check if your temporary table is cached.

* Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

* Partition by the "date_built" field on the formatted parquet home sales data.

* Create a temporary table for the parquet data.

* Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

* Uncache the home_sales temporary table.

* Verify that the home_sales temporary table is uncached using PySpark.

`
# Compare Run Times on Query 4 (q4)

* Uncache Runtime: 0.6964857578277588 seconds

* Cached Runtime: 0.4450709819793701 seconds

* Runtime with the parquet DataFrame: 0.48825621604919434 seconds`