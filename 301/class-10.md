# Readings: In Memory Storage

[Return to 301 TOC](301TOC.md)

## Understanding the JavaScript Call Stack

**[Reading from - Link](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)**

- **What is a ‘call’?** > A functon invocation (call).

- **How many ‘calls’ can happen at once?** > One active at a time. The call stack in single function(s) execution.

- **What does LIFO mean?** > Last In First Out.

- **Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.** >

```javascript
function firstFunction() {
  console.log("Hello from firstFunction");
}

function secondFunction() {
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();
```

The above copied from the requried reading source noted above with the link.

- **What causes a Stack Overflow?** > Recursive function (a function that calls itself) without an exit point from the stack to pop this function off the stack. The browser will throw a Maximum call size exceeded error.

## JavaScript Error Messages

**[Reading from - Link](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)**

- **What is a `refrence` error?** > Using a variable before it is declared.

- **What is a `syntax` error?** > When some code is wrong that cannot be parsed in terms of syntax.

- **What is a `range` error?** > When you try to manipulate an object (variable) beyond its boundaries like the length.

- **What is a `type` error?** > When the types (number, string, and so on) you are trying to use or access are incompatible.

- **What is a `breakpoint`?** >Pauses execution of your code at that line and shows you the debugger module to helpy see what state your code is at with all the variables and more at that point.

- **What does the word `debugger` do in your code?** > Allows you to specify a breakpoint from within your code. When code is ran, execution of the code will pause at this location.

### Things I want to know more about

- React Bootstrap or some other types of style libraries (Tailwind).
- Better understaind of this programming method of functional programming.
- Material UI
- Next.JS
- React Ionics

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
