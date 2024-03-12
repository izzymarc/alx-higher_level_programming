# SQL Basics

This project marks our initial exploration into relational databases. My focus has been on gaining proficiency with the basics of SQL, including creating and manipulating data within databases, crafting subqueries, and applying various functions.

## Assignments :page_with_curl:

* **0. Show all databases**
  * File: [0-list_databases.sql](./0-list_databases.sql) - A MySQL script to display all existing databases.

* **1. Generate a new database**
  * File: [1-create_database.sql](./1-create_database.sql) - A MySQL script to establish the database named `hbtn_0c_0`.
  
* **2. Erase a database**
  * File: [2-remove_databases.sql](./2-remove_databases.sql) - A MySQL script to remove the database called `hbtn_0c_0`.

* **3. Display all tables**
  * File: [3-list_tables.sql](./3-list_tables.sql) - A MySQL script to show all tables.
  
* **4. Create your first table**
  * File: [4-first_table.sql](./4-first_table.sql) - A MySQL script to construct a table named `first_table`.
  * Structure:
    * `id`: INT
    * `name`: VARCHAR(256)

* **5. Describe the full table**
  * File: [5-full_table.sql](./5-full_table.sql) - A MySQL script that provides a detailed description of `first_table`.
  
* **6. Show everything within a table**
  * File: [6-list_values.sql](./6-list_values.sql) - A MySQL script to list every row from `first_table`.

* **7. Insert your first record**
  * File: [7-insert_value.sql](./7-insert_value.sql) - A MySQL script to add a new record into `first_table`.
  * Details:
    * `id` = `89`
    * `name` = `Best School`

* **8. How many 89s?**
  * File: [8-count_89.sql](./8-count_89.sql) - A MySQL script that counts how many records have `id = 89` in `first_table`.

* **9. Complete creation**
  * File: [9-full_creation.sql](./9-full_creation.sql) - A MySQL script to both create and populate `second_table`.
  * Structure:
    * `id`: INT
    * `name`: VARCHAR(256)
    * `score`: INT
  * Entries:
    * `id` = 1, `name` = "John", `score` = 10
    * `id` = 2, `name` = "Alex", `score` = 3
    * `id` = 3, `name` = "Bob", `score` = 14
    * `id` = 4, `name` = "George", `score` = 8

* **10. Sort by best score**
  * File: [10-top_score.sql](./10-top_score.sql) - A MySQL script to sort `second_table` records by descending `score`.

* **11. Choose the top performers**
  * File: [11-best_score.sql](./11-best_score.sql) - A MySQL script to display records from `second_table` with a `score >= 10`, sorted by descending score.

* **12. No shortcuts**
  * File: [12-no_cheating.sql](./12-no_cheating.sql) - A MySQL script to update Bob's score to 10 in `second_table`.

* **13. Exclude the underperformers**
  * File: [13-change_class.sql](./13-change_class.sql) - A MySQL script to delete records from `second_table` with `score <= 5`.

* **14. Calculate the average**
  * File: [14-average.sql](./14-average.sql) - A MySQL script to find the average `score` in `second_table`.

* **15. Group by score**
  * File: [15-groups.sql](./15-groups.sql) - A MySQL script to list scores and the count of records sharing that score in `second_table`, ordered by descending count.

* **16. Exclude the unnamed**
  * File: [16-no_link.sql](./16-no_link.sql) - A MySQL script that lists records from `second_table` by descending `score`, omitting those without a `name`.

* **17. Switch to UTF8**
  * File: [100-move_to_utf8.sql](./100-move_to_utf8.sql) - A MySQL script that converts database `hbtn_0c_0` to use UTF8 encoding.

* **18. Average temperatures**
  * File: [101-avg_temperatures.sql](./101-avg_temperatures.sql) - A MySQL script to show the average temperature in Fahrenheit

 by city, sorted in descending order.

* **19. The hottest cities**
  * File: [102-top_city.sql](./102-top_city.sql) - A MySQL script to display the top three cities with the highest average temperatures during July and August, in descending order.

* **20. State temperature extremes**
  * File: [103-max_state.sql](./103-max_state.sql) - A MySQL script that lists the highest temperature by state, sorted by state name.
  
## Database Dump :dolphin:
* For tasks 101-103, queries are made against the [temperatures.sql](./temperatures.sql) database.