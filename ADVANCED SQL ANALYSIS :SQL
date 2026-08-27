-- ADVANCED SQL ANALYSIS
-- Remove duplicate values using DISTINCT
SELECT DISTINCT CITY
FROM SALES_TRANSACTIONS;


-- Find products starting with a specific letter
SELECT PRODUCT_NAME
FROM SALES_TRANSACTIONS
WHERE PRODUCT_NAME LIKE 'A%';


-- Find products containing a specific word
SELECT PRODUCT_NAME
FROM SALES_TRANSACTIONS
WHERE PRODUCT_NAME LIKE '%Phone%';


-- Find transactions between two unit prices
SELECT PRODUCT_NAME, UNIT_PRICE
FROM SALES_TRANSACTIONS
WHERE UNIT_PRICE BETWEEN 500 AND 1500
ORDER BY UNIT_PRICE;


-- Find transactions from selected cities
SELECT PRODUCT_NAME, CITY, UNIT_PRICE
FROM SALES_TRANSACTIONS
WHERE CITY IN ('Mumbai', 'Ahmedabad', 'Delhi');


-- Find transactions excluding selected cities
SELECT PRODUCT_NAME, CITY, UNIT_PRICE
FROM SALES_TRANSACTIONS
WHERE CITY NOT IN ('Mumbai', 'Ahmedabad');


-- Find records where payment mode is available
SELECT *
FROM SALES_TRANSACTIONS
WHERE PAYMENT_MODE IS NOT NULL;


-- Find records where payment mode is missing
SELECT *
FROM SALES_TRANSACTIONS
WHERE PAYMENT_MODE IS NULL;


-- Replace NULL payment mode with Unknown
SELECT
    PRODUCT_NAME,
    CITY,
    COALESCE(PAYMENT_MODE, 'Unknown') AS PAYMENT_MODE
FROM SALES_TRANSACTIONS;


-- Convert product names to uppercase
SELECT
    UPPER(PRODUCT_NAME) AS PRODUCT_NAME
FROM SALES_TRANSACTIONS;


-- Convert city names to lowercase
SELECT
    LOWER(CITY) AS CITY
FROM SALES_TRANSACTIONS;


-- Find length of product names
SELECT
    PRODUCT_NAME,
    LENGTH(PRODUCT_NAME) AS NAME_LENGTH
FROM SALES_TRANSACTIONS;


-- Remove extra spaces from city names
SELECT
    TRIM(CITY) AS CLEAN_CITY
FROM SALES_TRANSACTIONS;


-- Calculate sales and profit margin example
SELECT
    PRODUCT_NAME,
    QUANTITY,
    UNIT_PRICE,
    QUANTITY * UNIT_PRICE AS TOTAL_SALES
FROM SALES_TRANSACTIONS;
