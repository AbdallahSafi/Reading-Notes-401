# Event Driven Applications

__Why is access control important?__  
Access control is important to protect users. Without it, anybody would be able to access any part of a website, and they could access other users data and change other accounts in ways that would not be good for the user.  
__Describe an application that would need access control__  
News websites often have a mixture of free articles and subscription plans. There needs to be a way to make sure that a paying customer is on the website to access the premium content.
__What is a role used for?__  
A role defines what capabailities a user will have on a web application. For example, a guest may have limited access, and an admin would probably have full access.
__Why is role based access control more scalable than discretionary or mandatory access control?__  
Mandatory access control is powerful but it is difficult to implement and it requires a lot of maintainance. Discretionary access control is more flexible than mandatory, but it comes with a greater risk that data will fall into the wrong hands. RBAC is a good middle ground, where different users will be assigned their roles, and all of their access will be based on the role they have. It seems that this would make it easier to change the access of a certain role as it changes with this method.  

|Term | Definition |  
|---|---| 
| Authorization |  Used to determine the privileges and access to resources that a client has when using an app or network. It is preced by authentication.  |
| Role Based Access Control | Restricts network access based on a person's role. This allows some people to have limited access to a network and others to have full access, and eveything in between.|
| Capabilities | Capabilities are what a client can do in an application with their role. |