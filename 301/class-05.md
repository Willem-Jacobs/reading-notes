# React Readings

[Return to 301 TOC](301TOC.md)

## React - Putting it All Together

### React Docs - Thinking in React

**[Reading from - Link](https://reactjs.org/docs/thinking-in-react.html)**

- **How would you break a mock into a component hierarchy?** > Draw boxes around each component and subcomponent and give them names. This what you can determine to be components that will make up the entire model. Take into consideration the data flow. After components are identified, arrange them into a hierarchy.

- **What is the "single responsibility principle" and how does it apply to components?** > Where a component should ideally only do one thing. If it grows and does more, break it up.

- **What does it mean to build a "static" version of your application?** > A version of your app that takes your data model and renders the UI but has no interactifity. This to reuse other components and pass data using props. There is no state in your static version. This to test to flow of your app components. This a good way to test your prop passing and your one way data flow to keep everything modular and fast.

- **Once you have a static applicaiton, what do you need to add?** > State needs to be added next after your static model UI and props have proper flow.

- **What are the three questions you can ask to determine if something is state?** > 1. Is it passed in from a parent via props? 2. Does it remain unchanged over time? 3. Can you compute it based on any other state or props in your component?

- **How can you identify where state needs to live?** > The top component that needs the state in the hierarchy and has to pass the state value(s) down to children where each child shares that state along with needing it as props.

### Things I want to know more about

- None at this time.

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
