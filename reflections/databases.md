# Replace this with the lecture / discussion topic

I provided 3 topics as an example if there are 2 or 5 that your groups agrees on do not feel the need to have 3.

## Summarize the lecture / class discussion topics

### Relational Databases
A relational database is one that stores and provides access to data points that are related to one another in the database. Each row in the data is represented by a unique ID (key) which is used to map attributes of the column to one another. This database is optimized for storage, query, and compute and uses SQL to access the database. Types of RDMS: MySQL, PostgreSQL, Db2, etc.

### Document Databases
Document databases are NoSQL databases that store data in single "documents" that encapsulate the data all in one place in a standard format. These "documents" are queryable using key/id fetch, which allows for search optimization based on the contents of the document itself. This is in contrast to relational databases, which capture value related to a single object across several tables. 

### Graph Databases
Graph databases store nodes and relationships instead of tables / documents. In this paradigm, data is represented by nodes and relationships are the edges. Unlike relationship databases, all of the data is stored without restricting it to a pre-defined model, giving it increased flexiblity relative to relational databases. 

### NextGen Databases
We briefly discussed in class the next generation of databases - newSQL and real-time DBs. NewSQL attempts to combine the relationships from relational databases with the capacity and performance of document databases. Real-time DBs are built to be updated extremely quickly, and have time ranges of 'temporal validity'. 

## Identify the key implications and takeaways

### Relational Databases
The main benefit of Relational Databases is to be able to connect the tables to understand the relationship between data, identifying any meaningful insights that can be derived. In addition, this helps with better data management reducing redundancy and allowing for flexibility in changes to the data.

### Document Databases
Document databases allow for rapid search and are iterable. If a user changes information available in his or her document object, that can be updated in a single location rather than requiring the updating or creation of new tables. This type of database is flexible as to the type of data it stores, as well, allowing all relevant data for an object to be searched, updated, or analyzed in one place.

### Graph Databases
Graph databases are well optimized to better understand relationships without pushing a pre-defined model, making it popular for social media analytics. For example, we can quickly understand the relationships between users (e.g. friends) but also other attributes (e.g. location, company, etc.). In this way, it is possible to represent varied relationships across varied objects in a way that MySQL would struggle with, especially as a platform scaled further. 

### NextGen Databases
NewSQL databases are great for transactional data, where there are lots of data created in a short time frame, but the relationships are still important. Previously, large relational databases could only be maintained by improving the computer/server which required significant investment. NewSQL makes large relational databases possible for smaller companies with less resources. Real-time databases are particularly useful for banking, reservation systems, or medical records. Things that change quickly and frequently and will be accessed soon after a change are well-suited to real-time databases.

## What additional resources / links can deliver more in depth knowledge / thinking about the lecture / class discussion topic

### Relational Databases
Understanding the basics of relational databases: https://searchdatamanagement.techtarget.com/definition/relational-database

Choosing between databases: https://www.pluralsight.com/blog/software-development/relational-vs-non-relational-databases

Industry use of PostgreSQL: https://learnsql.com/blog/companies-that-use-postgresql-in-business/

### Document Databases
AWS has some good information on definitions and use cases for document databases, including here: https://docs.aws.amazon.com/documentdb/latest/developerguide/document-database-use-cases.html

This article by a data scientist also offers some perspectives on document databases:

https://www.linkedin.com/pulse/20141025163418-38485481-nosql-document-database-what-are-my-ideal-use-cases/

### Graph Databases
Graph databases are powerful tools to analyze relationships. Facebook created a TAO (The Associations and Objects) view of its data which enabled deeper and more advanced analytics without forcing them to adhere to the increasingly complex MySQL tables. https://neo4j.com/news/how-facebook-matured-its-data-structure-and-stepped-into-the-graph-world/

Another company that uses graph databases is Twitter as detailed here https://blog.twitter.com/engineering/en_us/a/2010/introducing-flockdb

### NextGen Databases
Basics on the differences in newSQL: https://www.dbta.com/Columns/DBA-Corner/What-Is-a-NewSQL-Database-System-104489.aspx

Very involved paper on real-time databases and possible applications: https://users.soe.ucsc.edu/~sbrandt/courses/Winter00/290S/rtdb.pdf
