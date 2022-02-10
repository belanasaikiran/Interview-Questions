# ReactJs

1. **What are the features of React?**
    - JSX
    - Components
    - One-way Data Binding
    - Virtual DOM
    - Simplicity
    - Performance
2. **What is JSX ?**
   
   
    JSX stands for JavaScript XML. 
    
    It is a React extension which allows writing JavaScript code that looks similar to HTML. It makes HTML file easy to understand. The JSX file makes the React application robust and boosts its performance. JSX provides you to write XML-like syntax in the same file where you write JavaScript code, and then preprocessor (i.e., transpilers like Babel) transform these expressions into actual JavaScript code. Just like XML/HTML, JSX tags have a tag name, attributes, and children.
    
    ```jsx
    ReactDOM.render(){
    return(
    <div>
    <h1> display something </h1>
    </div>
    )
    }
    ```
    
3. **Explain the working of Virtual DOM.**
   
    Virtual DOM works in three steps:
    
    1. Whenever any data changes in the React App, the entire UI is re-rendered in Virtual DOM representation.
    
    ![https://static.javatpoint.com/interview/images/react-interview-questions1.jpg](https://static.javatpoint.com/interview/images/react-interview-questions1.jpg)
    
    2. Now, the difference between the previous DOM representation and the new DOM is calculated.
    
    ![https://static.javatpoint.com/interview/images/react-interview-questions2.jpg](https://static.javatpoint.com/interview/images/react-interview-questions2.jpg)
    
    3. Once the calculations are completed, the real DOM updated with only those things which are changed.
    
    ![https://static.javatpoint.com/interview/images/react-interview-questions3.jpg](https://static.javatpoint.com/interview/images/react-interview-questions3.jpg)
    
4. **What is the difference between Real DOM and Virtual DOM?**
   
    The following table specifies the key differences between the Real DOM and Virtual DOM:
    
    The real DOM creates a new DOM if the element updates.
    
    | Real DOM | Virtual DOM |
    | --- | --- |
    | The real DOM updates slower. | The virtual DOM updates faster. |
    | The real DOM can directly update HTML. | The virtual DOM cannot directly update HTML. |
    | The virtual DOM updates the JSX if the element updates. |  |
    | In real DOM, DOM manipulation is very expensive. | In virtual DOM, DOM manipulation is very easy. |
    | There is a lot of memory wastage in The real DOM. | There is no memory wastage in the virtual DOM. |
    
5. **What is Props?**
   
    Props stand for "Properties" in React. They are read-only inputs to components. Props are an object which stores the value of attributes of a tag and work similar to the HTML attributes. It gives a way to pass data from the parent to the child components throughout the application.
    
6. **What is a State in React?**

The State is an updatable structure which holds the data and information about the component. It may be changed over the lifetime of the component in response to user action or system event. It is the heart of the react component which determines the behavior of the component and how it will render. It must be kept as simple as possible.

7. **What is an event in React?**

An event is an action which triggers as a result of the user action or system generated event like a mouse click, loading of a web page, pressing a key, window resizes, etc. In React, the event handling system is very similar to handling events in DOM elements. The React event handling system is known as Synthetic Event, which is a cross-browser wrapper of the browser's native event.

Handling events with React have some syntactical differences, which are:

- React events are named as camelCase instead of lowercase.
- With JSX, a function is passed as the event handler instead of a string.

8. **Is it possible for a web browser to read JSX directly?**


Web browsers can't read JSX directly. This is because the web browsers are built to read the regular JS objects only, and JSX is not a regular JavaScript object.

If you want a web browser to read a JSX file, you must transform the files into a regular JavaScript object. For this purpose, Babel is used.

9. **What is React Router?**

React Router is a standard routing library system built on top of the React. It is used to create Routing in the React application using React Router Package. It helps you to define multiple routes in the app. It provides the synchronous URL on the browser with data that will be displayed on the web page. It maintains the standard structure and behavior of the application and mainly used for developing single page web applications.

10. **Why do we need a Router in React?**

React Router plays an important role to display multiple views in a single page application. It is used to define multiple routes in the app. When a user types a specific URL into the browser, and if this URL path matches any 'route' inside the router file, the user will be redirected to that particular Route. So, we need to add a Router library to the React app, which allows creating multiple routes with each leading to us a unique view.

```jsx
<switch>  
      <h1>React Router Example</h1>  
      <Route path="/" component={Home} />  
      <Route path="/about" component={About} />  
      <Route path="/contact" component={Contact} />  
</switch>
```