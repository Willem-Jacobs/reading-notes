# React Readings

[Return to 301 TOC](301TOC.md)

## State and Props

### React Lifecycle

**[Reading from - Link](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)**

- **Based on the diagram, what happens first, the 'render' or the 'componentDidMount'?** > The 'render' happens before the componentDidMount
- **What is the very first thing to happen in the lifecycle of React?** > During the mounting phase, the constructor is the first item that runs.

- **Put the lifecycle items in order?** > contructor, render, React Updates, componentDidMount, componentWillUnmount.

- **What does componentDidMount do?** > Allows side effects and state upate along with a good locaiton to fetch data using http requests. Should the state change, a rerender is initiated as the state changed.

### React State Vs Props

**[Video from - Link](https://www.youtube.com/watch?v=IYvD9oBCuJI)**

- **What type of things can you pass in the props?** > Allows you to pass values from parent component to a child component. The values can be of any data type (strings, functions, objects, etc) but the child cannot change their props. The parent component remains the owner of the prop and the one that can change it.

- **What is the big difference between props and state?** > Props are read only values passed from a parent to a child to be used by the child and owned by the parent. Only the parent can change the value. The child can update it if the parent provided a callback function passed as a prop to the child and available in the child. This is an upstream change.

- **When do we re-render our application?** > When state is modified in any component from anywhere in the code.

- **What are some examples of things that we could store in state?** > State is handled and updated inside the component. State triggers a re-render. State is used to store values that updated and to cause a re-render. State values are also preserved during page changes re-render. Example is values from a form to be stored in states. Values of states are for inside the component to be maintained by the component. Values of state can be passed to child but they are passed as props.

### Things I want to know more about

- None at this time.

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
