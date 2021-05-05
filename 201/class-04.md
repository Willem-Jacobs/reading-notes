# HTML Book Readings

[Return to 201 TOC](201TOC.md)

*Resource: Duckett HTML Book* - Various parts cited from the resource

## Chapter 4 - Links (pp.74-93)

- Links are created using an `<a href="web address or page internal or #">LINK NAME</a>`.
- You can link to an external website using the full web address.
- You can link to other pages on your own website using the relative URL path. This where you specify the director (if needed) then the file name. If you need to move up you use `../` to move up a directory, add more `../` if needed then work your way down to the correct directory and specify the filename. Example `../../myfiles/index.html`.
- You can start up the user email program by using the `mailto:email@email.com` in the href attribute.
- You can force links to open in a new window by using the `target="_blank"` after the href attribute. (Should avoid this as many users do not like it). Let the user decide by right clicking on the link and then choosing to open in new tab or window.
- Finally, the last option is for tags on your own page if it is long. You have to specify `id` for the HTML elements and then you can use the `#` in the href to jump to that section. Example `<a href="#long_list">Jump to Long List</a>` and you have some element in your HTML that has the `id="long_list"` set.

## Chapter 15 - Layout (pp.358-404)

- Normal flow. `position:static` each block-level element sits on top of the next one. This the default way in which browsers display HTML elements.
- Relative positioning. `position: relative` moves an element in relation to where it would have been in normal flow. You then use `top, bottom, right, left` properties to move the element from where it would have been in normal flow. Values usually given in pixel, em, rem or percetage.
- Absolute positioning. `position: absolute` This takes the element box out of normal flow and no longer affets the position of other elements on the page. Using the properties of `top, right, bottom, left` you can position where the element should appear in relation to its containing element.
- Position fixed. `position: fixed`. This is a type of absolute positioning that positions the element in relation to the browser window. This keeps like a navigation bar title fixed and the other information scrolls behind it. You can use the offset properties of `top, right, bottom, left` to position the element. As the element is out of the normal flow, it allows other items to flow behind it but that element requires a margin-top to push it down so it is not hidden from the start.
- Overlapping elements. `z-index`. When using relative, fixed or absolute positioning, boxed can overlap and this can be controlled with the `z-index` property by setting a number. The higher the number the further to the front that item is.
- Floating elements. `float: right or left`. Allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. Anything else that sits inside that containing element will flow around the element that is floating. When using the float property, the width should be set for that element.
- Float used many times to float elements next to each other is a liquid flowing grid.
- Clearing Floats `clear: left, right, both, none` used to tell that the element assigned this should have no other element touching the side specified. This a way to force wrap and placement of floating elements.
- By using a float element along with width & margin you can create a multi column grid layout.
- With devices of many screen sized and resolution, the best design would be a liquid layout style.
- Liquid layout uses percentages to specify the width of each box so that the design will stretch to fit the size of the screen.
- CSS 3 does provide a grid layout but this chapter does not mention it. Instead it talks about using a CSS framework and then you just specify classes to setup and use the grid system. The one the book uses is 960 Grid System [link to 960 Grid](www.960.gs).
- Multiple stylesheets can be linked. You can use the standard `<link>` in the HTML file but can also import stylesheets from the CSS file using the `@import` property and setting the `url("filename");`

## Chapter 3 - (First part) Functions, Methods, and Objects (pp.86-99)

*Resource: Duckett JS Book* - Various parts cited from the resource.

- Function is a grouping of statements within a specified function name you create to perform a certain task. This function can take parameters and can return a single result if needed.
- A function can be reused to instead of repeating code over and over.
- Functions break up your code into smaller manageable chunks that you call (invoke) them as needed. Some may need additional parameters passed into the funciton to do some work and then return the result for you to use in the rest of your code.
- The syntax to create a basic function that takes no parameters and returns no value is as follows:

```
function myFunction() {
  console.log('My Function ran');
}
```

- The above function is then invoked when you need it by calling it using `myFunction()'`.
- Functions can take parameters that you pass into it by specifying names for the items being passed in between the ( ) seperated by a comma. The names specified is then used inside the body of the function to access them. Example `myFunction(firstName, lastName)`.
- Functions can return an item to the caller by using the `return` keyword at the end. Note that any statements after the `return` will never get called. The return is a variable that can be a single value, array, object or even another function.
- Keep in mind that variables declared inside the function are only available inside the function. This is the scope of how JS works.
- When calling a function that returns a value, you need to store that returned value into a variable and the calling method changes to `let myVariable = myFunction();`. This example will store the returned value from the `myFunction` into the `myVaribale` variable whish is outside the function thus making the value available to other parts of the code.
- Functions can be invoked before they are declared as JS will parse the code file looking for functions before starting execution. For this to work, the proper decleration method has to be used for a function that is named.
- Anonymous functions can also be used and these are functions stored in a variable. These can't be invoked before they are declared. Anonymous function look like `let myFunction = function() { console.log('Hello')};`. You can see that the function has no name but it is on the expression of the varibale and can be invoked by calling the varibale.
- An anonymous function can be invoked at the time of declaring it placing `()` directoy after the closing "}" and wrapping the entire function in `()` example:

```
let myVar = (function() {
  console.log('Hello");
}())
```

- Scope. Any varibale declared in a block of code surrounded by `{ }` will be scoped locally to that block only as long as you use the `let or const` keywords. These 2 methods of declaring will declare scoped variables. In constrast, `var` is not scoped and is globally available to everything in that code file.

## Article - 6 Reasons for Pair Programming

[Link to 6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

[Return to 201 TOC](201TOC.md)

[Reutrn to Main Page](../README.md)
