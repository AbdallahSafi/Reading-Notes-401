# `<Login />` and `<Auth />`

__Why is the Context API useful?__   
The Context API is useful because it can change important values for many components at once from a centralized location, without all of the values having to be passed through many layers of props.  

__Can a component outside of a provider get its context?__   
It needs to be in a provider, or in a component whose parent is wrapped in the provider.  

__What are some common use cases for using the Context API?__   
It can be used to show who is logged in and what authorizations they have.  

__Describe “Context Hell”__  
Without useContext, you many have to pass props through many layers of components to get info to the right place. This can be frustrating and can lead to easy to miss mistakes.  

|Term | Definition |  
|---|---|
| global state |  This is the state of the entire React application.|
| gloabl context | This is context that affects the entire application, and it will share data to everything in the React component tree.|
| provider | The context provider accepts a value that will be passed to its children. All children components will rerender when the value changes. |
| consumer | This is a React component that subscribes to context changes in value of the Provider.|  