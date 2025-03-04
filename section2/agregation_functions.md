# Patter Machine Operators

### Like Operator


The SQL LIKE operator is used to  search for a specified pattern in a column. Here’s how you can use it in your queries

`SELECT first_name, last_name, last_connection FROM users WHERE last_connection LIKE '221%'`

In the above example we are saying that we want **first_name**, **last_name** and **last_connection** WHERE **last_connection** starts with 221.


### Between operator

The Between operator in SQL is used to filter the result set by checking wheter a value lies within a specified range. It is inclusive, meaning both the lower and upper bounds are inlcuded in the result

**Example**

`SELECT first_name, last_name, followers FROM users WHERE followers BETWEEN 4600 AND 4700`

### MAX, MIN, COUNT, ROUND, AVG

Example

`SELECT MAX(followers) as max_followers, 
		MIN(followers) as min_followers,
		AVG(followers) as avg_follwers FROM users;`


### Count Function

The **Count()** Function in sql is an agregate function that return the number of rows or non-null values from a specified colums

### First example: 

`SELECT COUNT (*) as total FROM users WHERE followers >= 4600`

when we have a table like this:

|   name    | followrs | City       |
|-----------|-----|------------|
| Alice     | 4600  | New York   |
| Bob       | 4600  | Los Angeles|
| Charlie   | 4600  | Chicago    |


