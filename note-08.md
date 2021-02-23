# What is SQL?
SQL is a domain-specific language used in programming and designed for managing data held in a relational database management system, or for stream processing in a relational data stream management system.

![ds](https://techskill.sg/wp-content/uploads/2020/06/SQL-server.jpg)

To retrieve data from a SQL database, we need to write SELECT statements

```
SELECT column, another_column, …
FROM mytable;
```

If we want to retrieve absolutely all the columns of data from a table, we can then use the asterisk (*) shorthand in place of listing all the column names individually.

```
SELECT * 
FROM mytable;
```

### Queries with constraints
In order to filter certain results from being returned, we need to use a WHERE clause in the query.
And below are some useful operators that you can use for numerical data (ie. integer or floating point):

![dlkksj](https://programmersought.com/images/948/c658dd486945a773beec3f5f618197d4.png)

