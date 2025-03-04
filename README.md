# Base-de-Datos LABORATORIO 1
# EJERCICIO 1
1. Given the reviews table, write a query to retrieve all 3-star reviews using the SQL WHERE clause. Only display the user_id and stars columns.
    ---SELECT user_id, stars FROM reviews
       where stars = 3;
2. Your given a products table, which contains data about different Microsoft Azure cloud products. Output all the data, in all the columns.
    ---SELECT * FROM products;
3. Given the reviews table, write a query to retrieve all 3-star reviews using the SQL WHERE clause. Only display the user_id and stars columns.
    ---SELECT user_id, stars FROM reviews
       where stars = 3;
4. Let's practice using AND along with WHERE to filter Amazon reviews based on all 4 of these conditions:
   the review should have 4 or more stars
   the review ID is less than 6000
   the review ID is more than 2000
   the review can't come from user 142
    ---SELECT * FROM reviews
       where stars >= 4 AND review_id < 6000 AND review_id > 2000 AND user_id <> 142;
5. Imagine you are a Data Analyst working at CVS Pharmacy, and you had access to pharmacy sales data. Use the BETWEEN SQL command to find data on medicines:
   Which sold between 100,000 units and 105,000 units
   AND were manufactured by either Biogen, AbbVie, or Eli Lilly
   Output the manufacturer name, drug name, and the # of units sold.
    ---SELECT manufacturer, drug, units_sold FROM pharmacy_sales    
       WHERE units_sold BETWEEN 100000 AND 105000 
       AND (manufacturer = 'Biogen' OR manufacturer = 'AbbVie' OR manufacturer = 'Eli Lilly'); 
6. Imagine you are a Data Analyst working at CVS Pharmacy, and you had access to pharmacy sales data. Use the IN SQL command to find data on medicines:
   which were manufactured by either Roche, Bayer, or AstraZeneca
   and did not sell between 55,000 and 550,000 units
   Output the manufacturer name, drug name, and the # of units sold. for all the medicines which match that criteria.
    ---SELECT manufacturer, drug, units_sold FROM pharmacy_sales
       WHERE manufacturer IN ('Roche','Bayer','AstraZeneca')
       AND units_sold NOT BETWEEN 55000 AND 550000;
7. You have a table of 1000 customer records from a small-business based in Australia.
   Find all customers whose first name starts with "F" and the last letter in their last name is "ck".
    ---SELECT * FROM customers 
       WHERE customer_name LIKE 'F%' 
       AND customer_name LIKE '%ck'
       LIMIT 20;
8. You have a table of 1000 customer records from a small-business based in Australia.
   Find all customers where the 2nd and 3rd letter in their name is "e".
   Example: "Reece Smith"
    ---SELECT * FROM customers 
       WHERE customer_name LIKE '_e%'
       AND customer_name LIKE '__e%'
       LIMIT 20;
9. 
10.
11.
12.
13.
14.
15.
16.
17.
18.
19
20.

