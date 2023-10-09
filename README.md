# Home_Sales

The origial ipynb file was provided by UW Madison. 

First the necessary PySpark SQL functions were imported and the home_sales_revised.csv file was read in. 

A temporary table was created and I pulled from that origional table to be able to answer the asked questions. 

I then cached the previouslt created table and ran a query to filter or the view ratings with an average price od $350,000 or greater. Reran the same query again with the cached data. 

I partitioned on the date built and created a temporary table on the parquet data. Then ran the query again.  Once the runtimes were compared. 
  First one being .64 seconds. 
  Second one being .54 seconds. 
  Third one being 1.88 seconds. 

Finding that the cached runtime was faster than the uncached but the partitioned parquet data had a slower runtime.

  
I then uncached the temporary table and verified that the table was uncached. 

Finally downloading the Home_Sales.ipynb to this repository. 
