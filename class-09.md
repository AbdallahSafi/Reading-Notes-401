### API server:
**Application Programming Interface (API)** is a lightweight Web application that allows users to create and expose data APIs from data, without the need for custom development. Through simple point-and-click configuration, user can create and configure access from popular clients like Microsoft Power BI, Salesforce Lightning Connect, SharePoint External Lists, Excel, PowerPivot, and more.

### Router.param(name, callback)
Adds callback triggers to route parameters, where name is the name of the parameter and callback is the callback function. 

###### The parameters of the callback function are:

- **req**, the request object
- **res**, the response object.\
- **next**, indicating the next middleware function. The value of the name parameter. The name of the parameter.

#### Middleware
Middleware (also called pre and post hooks) are functions which are passed control during execution of asynchronous functions. Middleware is specified on the schema level and is useful for writing plugins.

#### Types of Middleware:
Mongoose has 4 types of middleware: document middleware, model middleware, aggregate middleware, and query middleware. Document middleware is supported for the following document functions. In document middleware functions, this refers to the document.

- validate
- save
- remove
- updateOne
- deleteOne
- init 

#### What is a Subdocument?
Subdocuments are similar to normal documents. Nested schemas can have middleware, custom validation logic, virtuals, and any other feature top-level schemas can use. The major difference is that subdocuments are not saved individually, they are saved whenever their top-level parent document is saved.