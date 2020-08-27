### Class 14 Reading
## Database Normalization

What is database normalization? It is the process of organizing a table into columns, and selecting what data is relevant. A table should contain specific data about a specific topic, and only data that supports that topic. Limiting the application of a table reduces data redundancies and related issues.

There are some general rules that can be used to help along with building effective normalized tables. Most of all -- scope. You don't want your table to have too many purposes. Tables should be easily modified if data changes; large, multipurpose tables make modification difficult and increase the possibility of errors.

There are three common database normalization forms:
1. 1st (1NF)
1. 2nd (2NF)
1. 3rd (3NF)

Per the article: 
"First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.

Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.

Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key."

These rules are *progressive* -- that is to say, 2NF depends on first satisfying 1NF. 3NF depends on 2NF and 1NF. You need 1 to have 2, and both 1 and 2 to have 3.