# Bearer Authorization
__Write the following steps in the correct order:__   
 - Register your application to get a client_id and client_secret
 - Ask the client if they want to sign in via a third party
 - Receive authorization code
  - Receive access token
 - Make a request to the access token endpoint  
  - Redirect to a third party authentication endpoint
 - Make a request to a third-party API endpoint

__What can you do with an authorization code?__  
Use an authorization code to get an access token. 

__What can you do with an access token?__  
Use the access token to gain access to the API or resource. 

__What’s a benefit of using OAuth instead of your own basic authentication?__  
This makes it easier for people visiting your site to log in, as they won't have to reenter all of their info, you will get it from another site.   


## Vocabulary Terms  
  
|Term | Definition |  
|---|---| 
|Client ID | The client ID is a public identifier for apps. It is generally stored as a hex string. h|
| Client Secret | The secret is only known to the application and the authorization server. It should be random and unguessable.|
| Authentication Endpoint | An HTTP endpoint that that clients can use to identify a user or obtain an authorization code that can be used to exchange for an access token. |
| Access Token Endpoint | This is where the app makes a request to get the access token for a user.|
| API Endpoint | This is one end of a communication channel with an API. This is the location where an API can get the resources it needs to carry out a function.  |
| Authorization Code | After the user returns to the client on the redirect URL path, the app gets the authorization code and can use it to get an access token. 
| Access Token | This allows an application to access an API. The app recieves an access token after the user is authenticated and authorized. |