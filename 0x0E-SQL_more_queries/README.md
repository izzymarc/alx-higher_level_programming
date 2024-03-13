# 0x0E. SQL - More queries

## About
This project delves into more advanced SQL queries, focusing on user and privilege management, working with multiple tables through various types of JOINs, and understanding the use of subqueries, UNION, and constraints. 

### Resources
- [How To Create a New User and Grant Permissions in MySQL](https://dev.mysql.com/doc/refman/8.0/en/creating-accounts.html)
- [How To Use MySQL GRANT Statement To Grant Privileges To a User](https://dev.mysql.com/doc/refman/8.0/en/grant.html)
- [MySQL constraints](https://dev.mysql.com/doc/refman/8.0/en/constraints.html)
- [Basic query operation: the join](https://dev.mysql.com/doc/refman/8.0/en/join.html)
- [SQL technique: subqueries](https://dev.mysql.com/doc/refman/8.0/en/subqueries.html)
- [SQL technique: join types](https://dev.mysql.com/doc/refman/8.0/en/join.html)
- [SQL technique: union and minus](https://dev.mysql.com/doc/refman/8.0/en/union.html)
- [MySQL Cheat Sheet](https://gist.github.com/hofmannsven/9164408)
- [The Seven Types of SQL Joins](https://www.codeproject.com/Articles/33052/Visual-Representation-of-SQL-Joins)
- [MySQL Tutorial](https://www.mysqltutorial.org/)
- [SQL Style Guide](https://www.sqlstyle.guide/)
- [MySQL 8.0 SQL Statement Syntax](https://dev.mysql.com/doc/refman/8.0/en/sql-syntax.html)

### Extra resources on relational database model design:
- Design
- Normalization
- ER Modeling

## Learning Objectives
- Creating a new MySQL user
- Managing privileges for a user to a database or table
- Understanding PRIMARY KEY and FOREIGN KEY
- Utilizing NOT NULL and UNIQUE constraints
- Retrieving data from multiple tables in one request
- Subqueries, JOIN, and UNION

## Requirements
- Use vi, vim, emacs as editors
- All files executed on Ubuntu 20.04 LTS using MySQL 8.0 (version 8.0.25)
- All SQL queries should have a comment just before (i.e. syntax above)
- All SQL keywords should be in uppercase (SELECT, WHERE…)

## More Info
- How to install MySQL 8.0 on Ubuntu 20.04 LTS
- Using “container-on-demand” to run MySQL

## Tasks
0. My privileges!
1. Root user
2. Read user
3. Always a name
4. ID can't be null
5. Unique ID
6. States table
7. Cities table
8. Cities of California
9. Cities by States
10. Genre ID by show
11. Genre ID for all shows
12. No genre
13. Number of shows by genre
14. My genres
15. Only Comedy
16. List shows and genres
