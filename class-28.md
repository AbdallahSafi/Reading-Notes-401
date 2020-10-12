# Component Composition

__Can a parent component access the state of a child component?__   
It seems to be possible to do this by lifting the state up. This way the state of the parent and child can be changed simultaneously.  

  
__What can be passed along in a prop variable?__   
Props can be numbers, strings, objects, arrays, functions. It seems that you can pass almost anything you need to move data around the app.  

 
__How can a child component “know” the state of another component?__   
They can trigger callback functions, and the parent component will pass the information as requested. It also seems that Redux helps with this.  
  

### Vocabulary
|Term | Definition |    
|---|---|  
| component props | These are passed from the parent compenent to children components, and they can be any type of data, including functions. |  
| component state | This is the state of a specific component. This will define what all the pieces of data and different parts of the page are at a given moment in time.|   
| application state | This is the state of the entire application, as different components may or not be in use at different times. |  

