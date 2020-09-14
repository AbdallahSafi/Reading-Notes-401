# Express

### Express Routing  
- Event Driven System  
    - `app.get('/thing', (request,response) => {})`  
- The Request Object  
    - `(request,...)`  
    - /:parameters  
    - Parameters can be passed along the url and accessed on the req.params object.  
        - `app.get('api/:thing',....)`  
            - `request.params.thing`  
    - Query Strings  
    - You can query the api be adding ? and a filter parameter and can be accessed on the req.obj.(name of filter)  
        - `http://server/route?ball=round`  
            - `request.query.ball`
- The Response Object  
    - `(..., response)`  
    - Responsible for sending information back to the browser  
    - Has `.send()` and `.status()` Express uses these to format the ouput to the browser  
    - Sends:  
        - Cookies  
        - Status Codes  

### Server Testing  
- Avoid starting the server to test  
    - Export it as a module in a library for testing  
- `SuperTest` is a 3rd party library that requires in your server and you can then run your tests on your server.  
    - This will hit your route as if the server was running  
- You can wrap `superagent` in a module  
    - Allows you to set up a 'mock' of this new agent module  
    - 
    
