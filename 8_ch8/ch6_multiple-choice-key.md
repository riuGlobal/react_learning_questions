
**Cool trick of ImmutableMap. Look at this piece of code

const ErrorMessage = ({ riu_word }) =>
ImmutableMap()
.set(null, null)
.get(
riuword,
(<button>{riu_word}</button>)
);

Here we are setting a constant to a function. This function retrieves the value of a set (the immutable map) getting the value associated to a key where the key is the argument "riu_word". 
What value is set to the constant when riu_word is null
**

*null. If rendered nothing will be rendered
- a button with no text
- null. If rendered, it will fail
- a button with no text. 

**Cool trick of ImmutableMap. Look at this piece of code

const ErrorMessage = ({ riu_word }) =>
ImmutableMap()
.set(null, null)
.get(
riuword,
(<button>{riu_word}</button>)
);

Here we are setting a constant to a function. This function retrieves the value of a set (the immutable map) getting the value associated to a key where the key is the argument "riu_word". 
What is set to the constant when riu_word='my button'
**

*a button with text:  mu button
-a button with text: riu_word 
-a button with no text
-nothing it will fail due to: Null pointer exception. 



**Can you initialize state with properties**
*yes
-no

**What is componentWillMount method?**

* Is a method that is called before the component is mounted.
- Is a custom method of the user that expressed the will to mount a component in the browser DOM. 
- Is method that mounts the component in the browser DOM.
-  Is a custom method of the user that expressed the will to mount a component in the React DOM.

**Looking at this code 

class UserListContainer extends Component {
state = {
data: fromJS({
error: null,
loading: null,
users: [],
}),
}
// Getter for "Immutable.js" state data...
get data() {
return this.state.data;
}
// Setter for "Immutable.js" state data...
set data(data) {
this.setState({ data });
}


componentWillMount() {

this.data = this.data
.set('loading', this.props.loading);
}
}



What are we doing inside the componentWillMount method?**

* Setting  value passed through props of loading to the value of state.loading
- Setting the String 'loading' to this.props.loading. 
- Setting the method loading to this.props.loading
- Setting the method loading to the state.loading


**what is shouldComponentUpdate() method for**
* Its used to decide whether a component should be re-rendered or not. This is used to have more effcient code. 
- Decides whether the values of state are updated with new values
- Its used to suggest wheter the component should  change at all. But wont do any operations and only log a message.
- Its used to decide whether the component should make any changes to state. It can set failure when it shouldnt update. 




**What is a noop?**
* NO-OPeration. A coding sentece that does nothing. 
- No-Object-Oriented-Programmin. Phylosphy used in react where all object oriented phylosophy is avoided.
- A React constant used to introduce breaks between paragraphs.
- NO-Over-Programming. React phylosophy of keeping a reduced amount of components but   large in code, since many components cause inefficency. 

**Imagine a scenario where we have code calling an API and the component callling it is unmounted. The API response will not found the component that called it. If we wish to avoid this we may use the lifecycle of the component. How?**

* We may use the componentWillUnmount and cancel the call to the api. Previously defining with a wrapper that will introduce a cancel method.
- We would never call an API from react
- We can avoid it, React does no validations
- we may use the shouldComponentUpdate and stop the API from returning an error. 




**Imagine scenario where we want to cancel a promise of a component that is unmounted. In this scenario a container component is the one that unmounted the component with the promise that was canceled. Do we need a reference to the promise canceled in the container component?**

* Yes. Otherwise we wont have a way to cancel it, we cant refer to it. 
- No, there is no way to cancel it anyways. 

