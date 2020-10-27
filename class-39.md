# Redux - Additional Topics 

__What's the best practice for "pre-loading" data into the store (onapplication start) in a Redux application?__   
The best practice is to wrap the opening preload in `useEffect`. With this, you need to take the function outside of the props that you passed into the component.  

__When using a thunk/async action that dispatches the actual action, which do you export from your reducer?__   
You will still be exporting the new data to replace the state from the reducer. The action calling the reducer will be sent as a function rather than an object.  

|Term | Definition |  
|---|---|
| middleware | In Redux, middleware provides a third-party extention point between the when an action is dispatched and the moment it reaches the reducer. It needs to be used for asynchronous calls with Redux.|
| thunk | Thunk is a redux middleware that allows you to do async functions in conjunction with Redux.|