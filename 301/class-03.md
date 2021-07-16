# React Readings

[Return to 301 TOC](301TOC.md)

## Passing Functions as Props

## Lists & Keys, Spread Operator, Lifting State

### React Docs - Lists and Keys

**[Reading from - Link](https://reactjs.org/docs/lists-and-keys.html)**

- **What does .map() return>?** > Maps over each element in the array returning a new array that meets the parameters you specify in the callback function that map requires. Map can be embedded in the JSX betweekn {} to run JS.

- **If I want to loop through an array and display each value in JSX, how do I do that in React?** > Use .map() on the array and return JSX part into a new array. Then output that array as JS in the render() return section.
  '''
  const numbers = [1, 2, 3, 4, 5]
  const displayNumbers = numbers.map(number => <li>{number}</li>);
  '''
  In the render return section:

'''

<ul>{displayNumbers}</ul>
'''

- **Each list item needs a unique?** > Key.

- **What is the purpose of a key?** > React uses this as an indentifier for the list item, or class instance to track what is to be updated/deleted. It is to provide a stable identity to the item. The value has to be unique among siblings.

### The Spread Operator

**[Video from - Link](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)**

- **What is the Spread Operator?** > for adding items to arrays, combining arrays or objects and spreading an array out into a function's arguments.

- **List 4 things that the spread operator can do?** > Spreads the array into seperate arguments. Addint an item to a list. Adding to state in React. Copy an array.

- **Give an example of using the spread operator to combine two arrays.** >
  '''
  const array1 = ['Hello', 'World'];
  const array2 = ['Goodbye', 'Tomorrow'];
  const arrayCombined = [...array1, ...array2];
  console.log(...arrayCombined);
  Output: Hello World Goodbye Tomorrow
  arrayCombined: ["Hello", "World", "Goodbye", "Tomorrow"]
  '''

- **Give an example of using the spread operator to add a new item to an array.** >
  '''
  const array1 = ['hello', 'everyone'];
  const newArray = [...array1, 'thank you'];
  Output of newArray = ['hello', 'everyone', 'thank you']
  '''

- **Give an example of using the spread operator to combine two objects into one.** >

### Video - How to Pass Functions Between Components

**[Video from - Link](https://www.youtube.com/watch?v=c05OL7XbwXU)**

- **n the video, what is the first step that the developer does to pass functions between components?** >

- **In your own words, what does the 'increment' function do?** >

- **GHow can you pass a method from a parent component into a child component?** >

- **How does the child component invoke a method that was passed to it from a parent component?** >

### Bookmark/Skim

**[React Tutorial through 'Declaring a Winner' - Link](https://reactjs.org/tutorial/tutorial.html)**
**[React Docs: Lifting State Up - Link](https://reactjs.org/docs/lifting-state-up.html)**

### Things I want to know more about

- None at this time.

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
