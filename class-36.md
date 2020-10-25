# Application State with Redux

__What are the advantages of storing tokens in “Cookies” vs “Local Storage”__  
Cookies are read server-side, and local storage is read client-side, so if the server needs the data, then it is better to use cookies.  

 
__Explain 3rd party cookies.__   
These are cookies tracked by websites other than the one you are currently visiting. For example, if you visit websites containing a certain product, it might save a cookie that other webistes can see, and you will see ads about that product in other places you are browsing.  

 
__How do pixel tags work?__   
This is a single transparent pixel added to a web page. This image is served from the ad server's domain so they can record cookies based on the users behavior while not relying on being seen or clicked on.  


|Term | Definition |  
|---|---|
| cookies | These are small files on a user's computer that hold data specific to a client and a website, which allow a webpage to be catered to a specific user.|
| authorization | People with different authorization levels have access to different parts of a system or network. First they are authenticated, then they authorized to go to different areas based on what they are allowed to see and do.|
| access control | This restricts access to different areas of a network based on a person's role in an organization. |
| conditional rendering | These are parts of a React app that will only be rendered in certain conditions. For example, in the app we worked on last week, the form was not rendered for users with 'read' access, but it was rendered for users with 'create' access. |
