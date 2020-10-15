# Routing 
__Do child components have direct access to props/state from the parent?__   
The parent can pass its state though props to the children, and can pass other children through props.children. 

__When a component “wraps” another component, how does the child component’s output get rendered?__
```html
<Main>
  <Content />
</Main>
```
With something like this, the Content component will be passed to the Main component as child.props, so it can used in the Main component.  

__Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?__   
It seems that is would be possible for a child component to also be used as a standalone component.  
__What trick can a parent use to share all props with it’s children?__   
You can do this with a spread operator. Put this in the parent compenent to pass all the props to a child component `<Child {...props}>`  



### Vocabulary
| Term | Definition |  
|---|---|
| props.children | This allows you to pass components as props and to use them in other components.  |  
| composition | This is where a specific component renders a more generic one and configures it with props. This is useful because sometimes you don't know what the children will be ahead of time.  h |  