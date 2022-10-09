Step 1: import the necessary module. Here I imported only one module called pandas which is a powerful tool for faster data analysis, data cleaning, and data pre-processing. 

Step 2: a quick EDA is performed to understand the pattern of the data. 

TASK 1: Products without prices 

Step 1:  for this task, I only used the columns “price_string” and  “product_type”.  there may be chance of having a value in price_string column for a nan value in product_type column, so deleting all the rows having nan value in product_type column is better (to find out the accurate count of Products with prices in the future). 

Step 2: fetch all the rows having zero dollar in price_string column. The products in the product type column will be the products without price. 


TASK 2: Count of products without prices and with prices in each Product Type, Category, Level 1  

 
Step 1: similar to task 1, the count of products that have no price will be the no.of rows in above table. 

Step 2: to find the count of products that have a valid price, fetch all the rows that don’t have zero dollar in price_string column. 

Step 3: repeat the step 1 and step 2 for category and level_1 column. Final result will be: 


TASK 3: Correct Product Prices in the correct format (eg: $56) wherever possible and separate them into currency and value columns. 

Step 1: for this task, I only used the column “price_string”. Then I cleaned the data by dropping all the NAN values in that column. 

Step 2: derived a new column called value from price_string. Removed the dollar sign from all the rows and converted the values into float. 

Step 3: added a column called “currency” which have value Dollar.  

Step 4: derived “cleaned_price_string” column from value column. edited Product Prices in the correct format (eg: $56) wherever possible. 


TASK 4: List out the categories with average price of product. 

Step 1: for this task, I only used the columns “price_string” and “categrory”. Since we are going to calculate the average price, I dropped all the NAN values in price_string column.  

Step 2: removed the dollar sign from the rows that have dollar sign in front and converted all the values into float. 

Step 3: calculated the mean by grouping category column. 

 
