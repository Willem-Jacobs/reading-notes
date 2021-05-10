# HTML Book Readings

[Return to 201 TOC](201TOC.md)

*Resource: Duckett JavsScript and JQuery interactive Front End Web Development* - Various parts cited from this resource

## Chapter 3 - Object Literals (pp.100-105)

- Objects are a grouping of variables and functions to represent a real world model.
- In an object variables become properties and functions become mehtods. Just different term used to define what they are but they are still created the same way. Just means the variables and functions and now part of an object.
- Variables in the object have a pairing of a key and a value. Same applies to functions where they have a key (the function name) then the function definition.
- The value of a property can be a string, number, boolean, array and another object. Methods are always functions but that function belowing to the object model.
- Defining an object is just about the same was a variable. The example below created a car object that contains the keys/value shown which are the properties and the method called detailedName.

```javascript
let car = {
  year: 2021,
  make: 'Ford',
  model: 'F150',
  detailedName: function() {
    return `${this.year} - ${this.make} - ${this.model}`
  }
}
```

- Accessing the values in this object is done by using the dot "." notation. Example:

```javascript
let myCarFullName = car.detailedName();
```

- The above will create a new variable called `myCarFullName` and assign it the value that is returned from the car model method called `detailedName` by first accessing the model then "." then the method name and invoking that method with the "()".
- The above are to create 1 object only as needed. This is an object literal.

## Chapter 5 - Document Object Model (DOM) (pp.183-242)

- Document Object Model (DOM) is a model of your rendered HTML page and is how JS can access and update the content on the web page from the browser.
- The browser creates a model of the tree in memory while it loads it.
- The model consits of 4 main nodes being Document Node, Element Node, Attribute Node and Text Nodes.
- All nodes but the text nodes can have children.
- Attribute nodes are not children but are part of the element. Just a different way of accessing them.
- Accessing elements is done with various JS commands: Note all begin with `docuemnt.`.
  - `getElementById()`
  - `querySelector()`
  - `getElementsByClassName()`
  - `getElementsByTagName()`
  - `querySelectorAll()`
  - `parentNode`
  - `previousSibling / nextSibling`
  - `firstChild / lastChild`
  - Text node has only 1 property to use to retrieve the value. The property is `nodeValue`.
  - Other properties that can be used to access to text content is `innerHTML` and `textContent`.
  - To access or update attribute values you use `className / id` lets you get or update the value of the class and ID attributes.
  - `hasAttribute()` is used to check if the element has attributes.
  - `getAttribute() / setAttribute() / removeAttribute()` are used for getting, setting and removing attributes from the element. You need to always check if the element has attributes first by using the `hasAttribute()` method
  - Your elements should be stored to variables if you need to work on that element more than once. Reminder that the variable stores a reference to where the node is in the DOM tree. You then run use the variable to access the element over and over and run the properties and methods of that element on the variable.
  - Node methods that are plural and `querySelectorAll` return a NodeList which is a collection of the node (similar to an array) even if it only finds one. The other methods return just 1 node.
  - Live & Static nodelists. When you want wo work with a nodelist several times, store it in a variable rather than quering it over and over.
    - A live NodeList will udpate the page and iteself at the same time. The methods that begin with `getElementsBy` return a Live NodeList.
    - A Static NodeList will udpate the page only. The NodeList is not updated to reflect the changes thus a query will need to be done again. The methods that begin with `querySelector` (which use CSS selector syntax) return Static NodeLists.
  - There are 2 ways to select an element from a NodeList. First being with the NodeList `item()` method and the second is same as accessing an array with the variable name then the `[index]` example: NodeList stored in variable called `elements` use the `let firstElement = elements[0]` to select the first element. First check the length of the NodeList before accessing any of the elements by using the `length` method on the NodeList variable.
  - You can use loops on NodeLists to repeat the tasks.
  - When you have a NodeList, you can "Traverse" the DOM by using these 5 properties:
    - parentNode
    - previousSibling
    - nextSibling
    - firstChild
    - lastChild
  - Most browsers treat whitespace between elements as a text node so the 5 properties listed above may not get you the result you expect.
  - Text Nodes you can use the `nodeValue` property to access text from the node. Used to get it and to set it.
  - Note that elements like `<em>` and others like this, will create a node for itself and then place the text for it in a child node of itself.
  - When working with an element node, rather than its text node, the element can contain markup. You have 3 properites that can be used:
    - `innerHTML` Gets/sets text & markup.
    - `textContent` Get/sets text only.
    - `innerText` Gets/sets text only.
  - The properites above will overwrite the entire contents of the element (both text and markup).
  - `textContent` ignores any markup inside the element and will replace the entire content of the element.
  - `innterText` should be avoided because of support, obeys CSS and performance.
  - `innterHTML` is a quick simple way to udpate markup and content in any element node. THere are security risks with using innerHTML and needs to be used with caution to not allow injection of malware code.
  - DOM manipulation methords are safer to use than `innterHTML` but require more code and can be slower.
  - 5 steps for DOM manipulation are:
    - Create new text node. `createTextNode()`.
    - Create new element node. `createElement()`.
    - Add node to element node. `appendChild()`;
    - Select element you want to add the new fragment to. Normal ways.
    - Append the new fragment to the selected element. `appendChild()`.
  - DOM manipluation can be used to remove elements from the DOM tree.
    - Store the element to be removed in a variable.
    - Store the parent of the element in a varibale.
    - Remove the element from its containing element with `removeChild()`.
  - `document.write()` is a simple way to add content that was not in the original source code to the page but it is rarely advised.
  - `innerHTML` lets you get and set the entire content of any element including markup as a string. Can be used to add a lot of markup using less code. Can be faster than DOM manipulation and is a simple way to remove all the content from an element by assigning it a blank string. Drawback has high security risk if the markup being added is not sanitized. Difficult to isolate single elements you want to update.

[Return to 201 TOC](201TOC.md)

[Reutrn to Main Page](../README.md)
