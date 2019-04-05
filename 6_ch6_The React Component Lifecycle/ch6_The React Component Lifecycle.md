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

null

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

a button with the text: my button

**Can you initialize state with properties**
yes

**Look at this code. 

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
// Called before the component is mounted into the DOM
// for the first time.
componentWillMount() {
// Since the component hasn't been mounted yet, it's
// safe to change the state by calling "setState()"
// without causing the component to re-render.
this.data = this.data
.set('loading', this.props.loading);
}
}

A UserListContainer component is defined and the method this.data.set is called within componentWillMount. What is component will mount method?
**

Is a method that is colled before the component is mounted as part of the lifecycle of a component. 

**Looking at the code of before. What are we doing inside the componentWillMount method?**

Setting the value of state.loading with the value passed through props of loading

**what is shouldComponentUpdate() method for**
Its used to decide whether a component should be rendered or not. This is used to have more effcient code. 

**What is a noop?**
No operation. A coding sentece that does nothing. 

**Imagine a scenario where we have code calling an API and the component callling it is unmounted. The API response will not found the component that called it. If we wish to avoid it we may use the lifecycle of the component. How?**

We may use the componentWillUnmount and cancel the call to the api. Previously defining with a wrapper that will introduce a cancel method. 

**Imagine scenario where we want to cancel a promise of a component that is unmounted. In this scenario a container component is the one that unmounted the component with the promise that was canceled. Do we need a reference to the promise canceled in the container component?**

 Yes. Otherwise we wont have a way to cancel it, we cant refer to it. 








