## Which of the following will accomplish using  inheritance  for inheriting state.

* Implement a base component with initial state and then extend from it. 
- Inheriting state is not desirable there for it actually will be avoided
- Using a method that react provides for inheriting state
- Best is to do it through external  library that provides  a method for inheritance.  

## How to inherit properties in React

* Implement a base and extend it
- Inheriting properties is not desirable there for is actually avoided
- Using a method that react provides for inheriting properties
- Use an external library with a method for inheriting properties



## Do PropTypes get inherited for validation

* Yes
- No

## How to extend JSX and Event handlers and have children classes define state

* Have a  base component with an element and extend it, then initialize state on the child class using componentWillMount
- Have a class define event handlers and call its methods from any class that requires them. Same can be done for JSX
- There are methods from the react-inheritance that will accomplish bith inheritance of JSX and of event-handlers
- There are external libraries that make  possible the inheritance of both jsx and event handlers. 


## What is a higher-order-function

* A function that takes a function as input and return another function
- A funciont that takes high-order parameters meaning components in React
- Any functional component
- A functional component that returns a component or anything renderable given some input.

## Look this code and explain what it is  accomplishing. 


import React from 'react';
export default (Component, predicate) =>
props =>
predicate() && (<Component {...props} />);




* A function that takes Component and predicate as input and returns:  a function that takes props  as input and returns jsx if predicate is true or nothing if predicate is false. Can be used for conditional rendering
- A function that takes Component, predicate, props as input and the executes predicate function and Component rendering. 
- A function that renders Component with props and executes a function predicate given whatever is defined in the argument predicate. 
- A functional component that will export the default Component and predicate function defined somewhere else in the component. 

## What is FLUX

* A set architectural patterns used to build large-scale React applications. 
- A react component that is used to specify common tasks for the flow of the lyfecycle
- A react library that is used to specify common tasks for the flow of the lyfecycle
- Flow, Lightweight, Unique, eXperience is a design technique that implements the  MVC (Model View Controller) design patter



 




