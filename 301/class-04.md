# React Readings

[Return to 301 TOC](301TOC.md)

## React Docs - Forms

## The Conditional (ternary) Operator Explained

### React Docs - Forms

**[Reading from - Link](https://reactjs.org/docs/forms.html)**

- **What is a “Controlled Component”?** > A component where React manages the state of the form so that the state of the React component is the “single source of truth”.

- **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why?** > As soon as they enter them. Why? To make the React component the single source of truth and to have the value available to pass to other components or rest from other event handlers

- **How do we target what the user in entering if we have an event handler on an input field??** > By reading the value from event.target.value. The value attribute on the element has to be set linked to the state property. The event handler has to be the onChange.

### The Conditional (ternary) Operator Explained

**[Reading from - Link](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)**

- **Why would we use a ternary operator?** > Shorter code.

- **Rewrite the following statement using a ternary statement**

```javascript
if (x === y) {
  console.log(true);
} else {
  console.log(false);
}

x === y ? console.log(true) : console.log(false);
```

### Bookmark/Skim

**[React Bootstrap - Forms - Link](https://react-bootstrap.github.io/components/forms/)**

**[React Docs - Conditional Rendering - Link](https://reactjs.org/docs/conditional-rendering.htmll)**

### Things I want to know more about

- None at this time.

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
