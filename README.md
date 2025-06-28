# Task-4-Aggregate-Functions-and-Grouping

This task demonstrates how to apply aggregate functions to summarize data and group results in SQL.

# Functions Used:
- SUM, COUNT, AVG
- GROUP BY, HAVING

Book
Columns: book_id, title, author, genre, price, published_year

Operations Performed:
Used aggregate functions like SUM(), COUNT(), AVG() on numeric columns (price, published_year)

Grouped data by genre and author

Filtered grouped data using HAVING

 Example Queries:
Total number of books:
select count(*) from Book;

Average book price:
select avg(price) from Book;

Total price of books per genre:
select genre, sum(price) as total_price from book group by genre;

Genres with average price > ₹300:
select genre, sum(price) as total_price from book group by genre having sum(price) > 300;

## Outcome:
Gained the ability to summarize and analyze book data effectively using SQL aggregate functions and grouping.

