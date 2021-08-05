# Readings: Functional Programming

[Return to 301 TOC](301TOC.md)

## Concepts of Functional Programming in Javascript

**[Reading from - Link](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)**

- **What is functional programming?** > Programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — [Wikipedia](https://en.wikipedia.org/wiki/Functional_programming)

- **What is a pure function and how do we know if something is a pure function?** > Returns the same result if given the same arguments. It does not cause observable side effects.

- **What are the benefits of a pure function?** > Stable, consistent and predictable. Given the same parameters, pure functions will always return the same result. Easier to test.

- **What is immutability?** > Data cannot change after it's created. If you want to cahnge an immutable object, you can't. Instead, you create a new object with the new value.

- **What is Referential transparency?** > A function that yields consistently the same result for the same input.

## Node JS Tutorial for Beginners #6 - Modules and require()

**[Video from - Link](https://www.youtube.com/watch?v=xHLd36QoS4k)**

- **What does the word ‘require’ do?** > Imports the specified file so the defined functions can be used in that file.

- **How do we bring another module into the file the we are working in?** > `const variableName = require('file name');` This imports the code file to be used and the item to be used is available under the varibaleName specified.

- **What do we have to do to make a module available?** > By doing a `module.export = variableName` This is the variable name you should use on the require and for the usage in the rest of the code that imports that file. Best practice.

### Things I want to know more about

- Better understaind of this programming method of functional programming.

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
