# Test Case

1. Can you create a simple Web Page which handles Multi-users login using MERN or other framework you are familiar with?
2. Can you create a simple Calculator using JS, HTML & CSS? 
3. Create a simple ToDo App which includes ReactJs as front end and handle requests with NodeJs in [Repl.it](http://Repl.it) ?
4. [Make a counter app that will increase the number of counts as users click on the “Add” button using Functional].(https://www.geeksforgeeks.org/differences-between-functional-components-and-class-components-in-react/#:~:text=Make%20a%20counter%20app%20that%20will%20increase%20the%20number%20of%20counts%20as%20users%20click%20on%20the%20%E2%80%9CAdd%E2%80%9D%20button%20using%20Functional%20and%20Class%20components)

Functional Components: Functional components are some of the more common components that will come across while working in React. These are simply JavaScript functions. We can create a functional component to React by writing a JavaScript function.

Syntax:
```
const Car=()=> {
  return <h2>Hi, I am also a Car!</h2>;
}
```
Example:
```
import React ,{useState} from "react";
 
const FunctionalComponent=()=>{
    const[count , setCount]=useState(0);
 
    const increase=()=>{
        setCount(count+1);
    }
 
    return
        <div style={{margin:'50px'}}>
            <h1>Welcome to Geeks for Geeks </h1>
            <h3>Counter App using Functional Component : </h3>
          <h2>{count}</h2>
            <button onClick={increase}>Add</button>
        </div>
    )
} 
 
 
export default FunctionalComponent;
```



5.  With your knowledge in front-end Web Technologies, Create a Web page similar to the following attached image. You can use any of your favourite frameworks or use plane HTML, CSS and Vannila Js. You can upload the code on repl.it and share us the link.

Refer - https://github.com/mohamadadithya/frontend-mentor-challenges/tree/master/sunnyside-agency-landing-page-main
