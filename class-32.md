# Custom Hooks 

__What does a component's lifecycle refer to?__  
This refers to the time from when a component mounts to when it unmounts. There are methods that you can call associated with this.  

__Why do you sometimes need to “wrap” functions in `useCallback` when called from within `useEffect`?__  
`useCallback` is nice because it fires a memoized version of the callback only if one of it's dependants has changed. This makes it faster and more efficient.  

__Why are functional components preferred over class components?__  
Functional components are less code, easier to read, perform better, and make it easier to separate components.  

__What is wrong with the following code?__  
```js
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```
`useEffect` should only be used with the count is changed in the code above, so it does not make sense for it to be in a `for` loop. `useEffect` should be outside of the `for` loop in this example.  

|Term | Definition |  
|---|---|
| State Hook | This is the same as using `this.state` in a class component, but can be used as a hook with a functional component. The state does not have to be an object unlike with class components.|
| effect hook | This hook tells React that you need to do something after render. Examples of things you could use this for include API calls or data fetching. It will by default run after every render. |
| reducer hook | This is similar to a state hook, but it returns the state paired with a dispatch method. This is preferable to state when you have complex state logic.|