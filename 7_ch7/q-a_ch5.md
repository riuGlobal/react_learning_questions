## Property validation. Does it enhance user experience or developmer expercience 

Developer, property validation will log warnings and fail rendering when getting unexpected input. User probably wont it even seeit since it 
will be removed on production. 

## What is fail fast?

Is an architectural property of software in whcih the system will crash completly rather than running with inconsistencies. 

## What is defensive coding. 

Is providing a way to handle errors and unexpected behaviour in order to avoid failure. 

## Is defensive coding desirable in react 

Is not since it will require imperative code and React has a pradigm for avoiding it in preference of descriptive coding. 

## What is 'any' useful for in property validation

To set a a structure and later change for the desired type and for using with for example 'isRequired' to indicate any type but required 

## What is the diference between Proptypes.element.isRequired and PropTypes.node.isRequired

element means a particular element of react, while node means anything that can be rendered. 

## PropTypes.instanceOf

requires an specific type 

## PropTypes.oneOfType 

takes as an argument an array of types like PropTypes.string, PropTypes.number and then controls wheter is a type of one of them. 

## control a specific value in array 

Use oneOf

## what is PropTypes.shape used for?

require a particular 'shape' for example the object passed should have a name filed of type String and an age of type integer. 

## Look at this code .This is a custom property validator can you explain what is happening 

**
myNumber: (props, name, component) =>
(Number.isFinite(props[name]) &&
props[name] > 0 &&
props[name] < 100) ? null : new Error(),};
**
 
wheter the prop has a myNumber that is a number that is between 1 and 99 both included 


