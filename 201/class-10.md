# HTML/JavaScript Book Reading

[Return to 201 TOC](201TOC.md)

## Chapter 10 - Error Handling & Debugging (pp.449-486)

*Resource: Duckett JavaScript and Jquery Book* - Various parts cited from the resource

- Finding errors in your code can be difficilt at times but by knowing how scripts are processed, the order in which statements are executed helps you out.
- Every statement in a script lives in one of three execution contexts:
  - Global Context - code that is in script but not in a function. There is only 1 global context in any page.
  - Function Context - Code that lives in a function and is only ran when called.
  - Eval Context - Exection of text treated like an internal function.
- The first 2 exection context correspond with the notion of scope being:
  - Global Scope - Variables declared outside a function are global to the page.
  - Function Level Scopt - Variables that live only inside the function and to get them out have to return them to the Global Context.
  - JS uses an exection stack running one line of code at a time and when a function needs data from another, it stacks it ontop of the waiting funcitons.
  - Execution context & hoisting. This relates to understanding how JS prepares the code file and then executes it. Prepare will read the file to create the scope, variables, functions and arguments and sets the value of `this` keyword. Execute will assign values to variables, reference functions and run their code by executing statements. This like hoisting variables and functions to the top of the code file or execution context so they are ready to be used.
  - When JS encounters an error, it will throw an exception and stops execution but will look for exception-handling code written by the programmer. It will look for the error handling code in the function that caused the error to be thrown. If not found there, it will look to its parent and so on all the way to the top global context.
  - Throwing an error created an Error Object that has valuable information in it. Like any other object, this is in an property/value pair.
  - There are 7 types of error objects available:
    - Error Object - Generic error - all others based upon this error
    - SyntaxError Object - Syntax that has been followed
    - ReferenceError Object - Tried to reference a variable that is not declared/within scope
    - TypeError Object - Unexpected datat type that cannot be coerced
    - RangeError Object - Numbers not in acceptable range
    - URIError Object - EncodeURI(), decodeURI() and similar methods used incorrectly
    - EvalError Object - eval() function used incorrectly
  - Deal with errors by debugging your code using the tools available in the browser or to handle errors gracefully using the the `try catch throw finally` statements.
  - Notes not completed. Not feelign well tonight and cutting it short. Will udpate them and add the rest as I also need to work on the career project.

[Return to 201 TOC](201TOC.md)

[Return to Main Page](../README.md)

