### Advanced Mongo/Mongoose

**Why would a developer choose to make data models?**

Before adding data to a database, a developer would need to assess how to structure their schema (in the case of a SQL database) or how they would set up information within a collection (in the case of a NoSQL database).  By making a data model, the developer would be able to get a handle on what data they are dealing with and what would be the most useful way of organizing that data within a database so that they can have a plan for what that database will actually look like.

**What purpose do CRUD operations serve?**

CRUD (Create, Read, Update, and Delete) describes the four functions that are necessary in any application that involve a database.  This means that the application should allow one to create new entries in the database, access the information within the database, alter/update the information in the database, and remove entries from the database as needed.  Without CRUD, one would not have full access to the database that they are interacting with.



**What kind of database is Postgres? What kind of database is MongoDB?**

* Postgres is a SQL database (specifically, an open source object-relational database system).

* MongoDB is a NoSQL database (specifically, a document-based distributed database)



**What is Mongoose and why do we need it?**

Mongoose is an Object Document Mapper that allows one to define objects with a strongly-typed schema that is mapped to a MongoDB document.  My understanding at this time is that while Mongoose is not strictly necessary to use MongoDB, it can help to bridge the gap between SQL and NoSQL data by mapping a user-defined schema onto a Mongo document.



**Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.**

In animal classifications, an Order is within a Class and contains many types of Family 



**Name 3 cloud based NoSQL Databases**

* MongoDB

* CouchDB

* Cassandra DB



---

### Definitions


|Term|Definition|Source|
|:--|:-:|--:|
|database|A data structure that stores organized information|https://techterms.com/definition/database|
|data model|An abstract model that organizes elements of data and standardizes how they relate to one another and ot hte properties of real-world entities|https://en.wikipedia.org/wiki/Data_model|
|CRUD|Short for Create, Read, Update and Delete - the four basic functions that models should be able to do at a bare minimum.|https://www.codecademy.com/articles/what-is-crud|
|schema|The skeleton structure that represents the logical view of the entire database - defining how data is organized and how the relations among them are associated|https://www.tutorialspoint.com/dbms/dbms_data_schemas.htm|
|sanitize|To remove illegal characters from data, for the purpose of protection from malicious data|https://medium.com/@abderrahman.hamila/what-sanitize-mean-and-why-sanitize-in-code-data-5c68c9f76164|
|Structured Query Language (SQL)|A language that allows one to write database queries.  These databases use a schema and store data in tables|https://www.youtube.com/watch?v=ZS_kXvOeQ5Y|
|Non SQL (NoSQL)|Database based on collections with associated documents - unlike tables, documents do not use a schema and there are not relations (relational data would need to be merged manually) because the documents are able to hold all the necessary data.  This allows for more flexibility of data|https://www.youtube.com/watch?v=ZS_kXvOeQ5Y|
|MongoDB|'humongous' - a NoSQL database meant to store large amounts of data|https://www.youtube.com/watch?v=ZS_kXvOeQ5Y|
|Mongoose|An ODM library for MongoDB and Node.js which manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB|https://www.freecodecamp.org/news/introduction-to-mongoose-for-mongodb-d2a7aa593c57/|
|record|A database entry that may contain one or more values|https://techterms.com/definition/record|
|document|Within a NoSQL database, a document is a record that contains data.  Documents live within a collection|https://docs.mongodb.com/manual/reference/glossary/|
|Object Relation Mapping (ORM)|A programming technique in which a metadata descriptor is used to connect object code to a relational database|https://www.techopedia.com/definition/24200/object-relational-mapping--orm|

---

