# Props and State

__Does a deployed React application require a server?__  
You do not need a server with a deployed React application.  

__Why do we prefer to test a React application at the behavior rather than the unit level?__  
This is important because of what we are doing with React. We need to know that it is behaving correctly to know that is is working, and we can do this with react-testing-library.  

__What does `npm run build` do?__   
This command creates a build directory with a production build of the app.  

__Describe the actual composition/architecture of a React application__  
There is a compenent hierarchy in a React app. Each component should match one piece of dat ain the application. Data flows down the component hierarchy.  

### Vocabulary
|Term | Definition |  
|---|---|  
| BDD | Stands for behavioral driven development. We run tests with React that will work with DOM nodes and find buttons, links, and text to make sure the page is behaving properly. |  
| Acceptance Terms | This is a type of testing that tests an application for acceptability. The goal is to make sure that the application meets all the requirements. |  
| mounting | This means putting elements in the DOM. The built in methods called are `constructor()`, `getDerivedStateFromProps()`, `render()`, and `componentDidMount()`   |  
| build | React apps are built. Writing a react app is called building.|  


