

# Company Analysis (Northwind)

>We are taking this opportunity to analyze Northwind Traders, importer and exporter of specialty food from and to around the world. We will be performing analysis on the company's performance utilizing their sales [datasets](/Northwind_Dataset.sql).

| No  |      Table_Name      | # of Rows |                                                       Description                                                        |
| --- | -------------------- | --------- | ------------------------------------------------------------------------------------------------------------------------ |
| 1   | Categories           | 8         | List of Category ID and names along with detailed description                                                            |
| 2   | Customers            | 91        | Comprehensive list of Northwind Trader's customers, from customer IDs, company names, addresses and contacts information |
| 3   | Employees            | 9         | List of Northwind Trader's employees: Names, birthdays, hire dates, contact information and addresses                    |
| 4   | Employee Territories | 49        | List of territory ID and related employee                                                                                |
| 5   | order_details        | 2,155     | List of products sold, from order IDs, product IDs, prices, quantity sold and discounts                                  |
| 6   | orders               | 830       | Customer and shipping details per order, from order IDs, customer IDs, order dates, shipped dates to shipping addresses  |
| 7   | products             | 7         | list of present and past products                                                                                        |
| 8   | region               | 4         | Region descriptions and their IDs                                                                                        |
| 9   | shippers             | 6         | Shipping companies's names, IDs and contact information                                                                  |
| 10  | suppliers            | 29        | detailed list of suppliers, from supplier IDs, company names, addresses, contact information                             |
| 11  | territories          | 53        | list of territory IDs, region IDs and their description                                                                  |
| 12  | usstates             | 51        | list of US states, assigned IDs, state abbreviation and region                                                           |

## Table of Content

## Relationship Diagram:
<p align="center">
    <img width=60% height=60%" src="/Images/Relationship_Diagram.png">


## Analysis (Role playing as an analyst in the company)
1. Prior to the annual review of Northwind's pricing strategy, Product team wants to look at the products currently being offered, we were asked to provide list of:

A. Product name
B. Product unit price

With the following conditions:

A. Unit price is between $10 and $50
B. Products are not discontinued

<details>
<summary>
Query
</summary>

2. Logistic team wants to conducts analysis of their performance in 1997, to identify which countries didn’t perform well. They asked us to provide them the list of countries with the following information:

A. Average days between order date and shipping date
B. Total number of unique orders (based on order id) 

Filtered based on the following conditions:
 
A. Order date is in 1997
B. Average days between order date and shipping date is >= 3 days but < 20 days 
C. Total number of orders is greater than 5

Order the results by average days between the order date and the shipping date in descending order.

<details>
<summary>
Query
</summary>

3. People Operation team wants to know the age of each employee when they first join the company and their current manager. We are tasked to provide them with a list of all employees including:

A. Full name
B. Job title
C. Age (at the time of joining the company)
D. their tenure in years until current date
E. Manager's full name
F. Manager's job title

Order the results by employee age and employee full name in ascending order (lowest first).

<details>
<summary>
Query
</summary>

4. Again, Logistics Team asked for our help to analyze their global performances from 1996 to 1997, to identify which month they perform well. We need provide them a list with:

A. Year/month in a single cell in a date format
B. Total number of orders
C. Total freight (formatted to have no decimals)

Filtered based on the following conditions:

A. Order date is from 1996 to 1997
B. Total number of orders greater than 20 orders
C. Total freight is greater than 2500

Order result by total freight in descending order

<details>
<summary>
Query
</summary>

5. Pricing Team wants to analyze which products had experienced price increases not in between 10% and 30%. We need to provide them a list of products including:

A. Product name
B. Current unit price
C. Initial/Previous unit price
D. Percentage increase

Filtered based on the following conditions:

A. Percentage increase is not between 10% and 30%
B. Finally order the results by percentage increase (ascending order).

<details>
<summary>
Query
</summary>