# Redux - Combined Reducers

__Why choose Redux instead of the Context API for global state?__  
Redux is the industry standard for managing state of large applications, so it is important to know well. It is more optimized for larger projects, because the context API rerenders more often.  

__What is the purpose of a reducer?__  
We need reducers to tell the application how to change state in response to an action. The action does not do anything except describe what happended and it is up to the reducer to respond to this.  

__What does an action contain?__  
An action contains a type and whatever payload you want it to have. There is flexibility in what there is besides the type.  

__Why do we need to copy the state in a reducer?__  
The reducer needs to be a pure function without any side-effects. It should only take in an action and return the new state, but it should not mutate the state, so we need to copy it to update it.  


|Term | Definition |  
|---|---|
| immutable state | This allows the state to only change when absolutely necessary to make React apps perform as well as possible.|
| time travel in redux | This is a feature of redux dev tools that allows you to see every state that a page has been in.|
| action creator | Actions send data from your application to your store, and are the only source of information for the store. An action creator is a function that creates an action. |
| reducer | Reducers tell the application how to change state in response to an action. |
| dispatch | This is the name of the function you use to send actions to the store. |