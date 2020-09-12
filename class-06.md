# HTTP and REST

### Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.

For university:
- there is student, Study major and Faculty.
- each Student has Study major and belongs in a Faculty

### What is the advantage of an ORM, like Mongoose?
- They write correct and optimized SQL queries, thereby eliminating the hassle for developers.

- They make the code easier to update, maintain, and reuse as the developer can think of, and manipulate data as objects.

- ORMs will shield your application from SQL injection attacks since the framework will filter the data for you!.

- ORMs provide the concept of Database Abstraction which makes switching databases easier and creates a consistent code base for your application.

### How does the repository pattern compare with an ORM?

Repositories deal with Domain/Business objects (from the app point of view), an ORM handles db objects. A business objects IS NOT a db object, first has behaviour, the second is a glorified DTO, it only holds data.

### When making a repository/facade, what flexibility do you gain?

The flexibility comes with if you need to move to another database layer later, you can code to an interface and then your application does not care what that initialization of that database layer is. It also makes testing a lot easier because then you can have a "TestingUsersRepository" that doesnt rely on anything but the class itself and your favorite js unit testing framework.

### Name 3 cloud based NoSQL Databases

1. Amazon Web Services
2. Azure by Microsoft
3. Garantia Data

## Document the following Vocabulary Terms

- **lifecycle** Application Lifecycle Management (ALM) is the specification, design, development and testing of a software application. ALM covers the entire lifecycle from the idea conception, through to the development, testing, deployment, support and ultimately retirement of systems.

- **collections** Collections are analogous to tables in relational databases.

- **the “Repository” design pattern** is one of the most popular design patterns to achieve such separation between the actual database, queries and other data access logic from the rest of the application.

- **mongoose middleware** are functions which are passed control during execution of asynchronous functions. Middleware is specified on the schema level and is useful for writing plugins.

- **Object Relation Mapping (ORM)** is the idea of being able to write queries like the one above, as well as much more complicated ones, using the object-oriented paradigm of your preferred programming language.

## HTTP

* HTTP stands for *Hyper Text Transfer Protocol*, a stateless request-response application layer protocol

  - Applications built using HTTP subscribe to the client-server computing model

  - **server**: host designed to provide a service
  - **client**: hosts that make requests to the service

## HTTP Requests

 * The first line of a request contains a **method**, **URL**, and **HTTP version**.  Following lines are request **headers**.

 *Key Terms regarding Methods*:

 **safe**: does not change the state of the server - should only be used for information retrieval

 **idempotent**: identical requests of this type will get identical responses, no matter how many times they are called.  All *safe* methods are also *idempotent*

 **cacheable**: the client is able to cache the response

 |HTTP Method|Request has Body|Response has Body|Safe|Idempotent|Cachable|
 |:--|:-:|:-:|:-:|:-:|:-:|
 |GET|no|yes|yes|yes|yes|
 |HEAD|no|no|yes|yes|yes|
 |POST|yes|yes|no|no|yes|
 |PUT|yes|yes|no|yes|no|
 |DELETE|no|yes|no|yes|no|
 |CONNECT|yes|yes|no|no|no|
 |OPTIONS|optional|yes|yes|yes|no|
 |TRACE|no|yes|yes|yes|no|
 |PATCH|yes|yes|no|no|no|

## HTTP Response

 * The first line of a response contains an **HTTP version**, **status code** and **status message**.  Following lines are request **headers**.

## REST

* Acronym for REpresentational State Transfer - a means by which we can reference, manipulate and transfer state.

|REST Method|CRUD Operation|Function|
|:-:|:-:|:--|
|GET|READ|Retrieve 1+ Records|
|POST|CREATE|Create a New Record|
|PUT|UPDATE|Replace Record with an updated version|
|PATCH|UPDATE|Replace the updated portion of the Record|
|DESTROY|DELETE|Remove a Record|

## [What Is A RESTful API? Explanation of REST & HTTP](https://www.youtube.com/watch?v=Q-BpqyOT3a8)

**API**: Application Program Interface - a contract provided by one piece of software to another (request & response)

