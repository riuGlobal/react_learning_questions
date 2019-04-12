## Which of the following will accomplish using  inheritance  for inheriting state.

* Implement a base component with initial state and then extend from it. 
- 

## How to inherit properties

Implemnet a base and extend

## Do PropTypes get inherited for validation

Yes

## How to extend JSX and Event handlers and have children classes define state

A base component with the element extend it and initialize state using componentWillMount

## What is a higher-order-function

A function that takes a function as input and return another function

## Look this code and explain what it is  accomplishing. 

<h1>
import React from 'react';
export default (Component, predicate) =>
props =>
predicate() && (<Component {...props} />);

</h1>


Returns a function taht takes props and return jsx if predicate is true or nothing if predicate is false. Can be used for conditional rendering

## What is FLUX

A set architectural patterns used to build large-scale React applications. 



 




