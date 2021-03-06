# React Readings

[Return to 301 TOC](301TOC.md)

## Passing Functions as Props

## Lists & Keys, Spread Operator, Lifting State

### React Docs - Lists and Keys

**[Reading from - Link](https://reactjs.org/docs/lists-and-keys.html)**

- **What does .map() return>?** > Maps over each element in the array returning a new array that meets the parameters you specify in the callback function that map requires. Map can be embedded in the JSX between {} to run JS.

- **If I want to loop through an array and display each value in JSX, how do I do that in React?** > Use .map() on the array and return JSX part into a new array. Then output that array as JS in the render() return section.

  ```javascript
  const numbers = [1, 2, 3, 4, 5] const displayNumbers = numbers.map(number => <li>{number}</li>);
  ```

  In the render return section:

  ```html
  <ul>
    {displayNumbers}
  </ul>
  ```

- **Each list item needs a unique?** > Key.

- **What is the purpose of a key?** > React uses this as an identifier for the list item, or class instance to track what is to be updated/deleted. It is to provide a stable identity to the item. The value has to be unique among siblings.

### The Spread Operator

**[Video from - Link](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)**

- **What is the Spread Operator?** > for adding items to arrays, combining arrays or objects and spreading an array out into a function's arguments.

- **List 4 things that the spread operator can do?** > Spreads the array into separate arguments. Add it an item to a list. Adding to state in React. Copy an array.

- **Give an example of using the spread operator to combine two arrays.**

  ```javascript
  const array1 = ['Hello', 'World'];
  const array2 = ['Goodbye', 'Tomorrow'];
  const arrayCombined = [...array1, ...array2];
  console.log(...arrayCombined);
  Output: Hello World Goodbye Tomorrow
  arrayCombined: ["Hello", "World", "Goodbye", "Tomorrow"]
  ```

- **Give an example of using the spread operator to add a new item to an array.**

  ```javascript
  const array1 = ['hello', 'everyone'];
  const newArray = [...array1, 'thank you'];
  Output of newArray = ['hello', 'everyone', 'thank you']
  ```

- **Give an example of using the spread operator to combine two objects into one.**

  ```javascript
  const object1 = {firstName: 'Bob'};
  const object2 = {lastName: 'Smith'};
  const object3 = {...object1, ...object2}
  Output of object3 = {firstName: 'Bob', lastName: 'Smith'}
  ```

### Video - How to Pass Functions Between Components

**[Video from - Link](https://www.youtube.com/watch?v=c05OL7XbwXU)**

- **In the video, what is the first step that the developer does to pass functions between components?** > Create the method in the component where the state to be changed is to pass this function to the child.

- **In your own words, what does the 'increment' function do?** > There are 2 'increment' functions. One in the child. One in the parent that manages the state. In the parent, it loops over each element in the object to find the matching name and then updates the count of the state for that person. In the child, it updates the local state of the child to display a banner at each object displayed level.

- **How can you pass a method from a parent component into a child component?** > Same as you pass props. Provide a name and a reference to the method. If method called 'increment' you would pass it with `increment={this.increment}`

- **How does the child component invoke a method that was passed to it from a parent component?** > By calling the prop related to the method in the parent. So, if you have a prop being passed called increment, the child would call `this.props.increment()` if any values need to be passed to the method in the parent, you would just add them like and other function/method being called.

### Bookmark/Skim

**[React Tutorial through 'Declaring a Winner' - Link](https://reactjs.org/tutorial/tutorial.html)**

**[React Docs: Lifting State Up - Link](https://reactjs.org/docs/lifting-state-up.html)**

### Things I want to know more about

- None at this time.

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
