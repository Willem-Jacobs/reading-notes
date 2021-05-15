# HTML/JavaScript Book Reading

[Return to 201 TOC](201TOC.md)

## Chapter 6 - Tables (pp.126-145)

*Resource: Duckett HTML Book* - Various parts cited from the resource

- Tables are use on an HTML page when needing to display data in a grid like manner that includes header top lines for columns and header for rows then you have cells that represent the data. Similar to a spreadheet.
- The basic structure of a table is defined below:

```HTML
<table> // defines a table
  <tr> // defines the table row
    <th></th> // table heading (blank cell)
    <th scope="col">Name</th> // heading for a column
    <th scope="col">Age</th> // heading for a column
  </tr>
  <tr>
    <th scope="row">Student A</th> // defines the row name
    <td>John Smith</td> // row data for column 1 (name)
    <td>40</td> // row data for column 2 (age)
  </tr>
  <tr>
    <th scope="row">Stduent B</th> // defines the row name
    <td>Jane Doe</td> // row data for column 1 (name)
    <td>28</td> // row data for column 2 (age)
  </tr>
</table>
```

- Above example the scope attribute on the `<th>` is used to define if the table header as a column or a row.
- The attribute of `colspan="##"` can be applid to a `<td>` to span multiple columns by providing the number of columns to span. You can also use `rowspan="#"` to make the column span across multiple rows.
- CSS can be added to each alement as needed using the normal selction/class/ID methods used to select HTML elements.
- `<thead></thead>, <tbody></body>, <tfoot></tfoot>` can be used to wrap parts of the table to define a head, body and footer sections then place the normal elements defined above between them.

## Chapter 3 - Functions, Methods, and Objects (pp.106-144)

*Resource: Duckett JavsScript and JQuery interactive Front End Web Development* - Various parts cited from this resource

- Constructor is a special function you define that acts as a model or blueprint to create new objects. The benefit of this over an object literal is you define the model once and reuse it for each object.
- Unwritten rule is to name to constructor with a capital letter as the start to indicate this is a constructor model.
- The values that the object will need are passed into the funciton like a normal function. Each property definition inside has to start wit hthe `this` keyword and the line ends with a `;` instead of a `,`.
- Additional properties can be added to the created object as usual way by just adding it. The below example shows a method that is available to the object that will add a miles property.

```javascript
function Car(make, model, year) {
  this.make = make;
  this.model = model;
  this.year = year;
  this.setMiles = function(miles) {
    this.miles = miles;
    return miles;
  }
}
```

- When needing to create an object based on the constructor, you create it using the `new` keywoard along with the constructor name after and passing in the values needed by the constructor to create the object.
- Using the above example, creating an object from this constructor you would use: `const car1 = new Car('Ford', 'F-150', 2020);`. This is create a new object called car1 with the properties passed in along with the setMiles method. When this method is called passing in the value of miles, a new property is added only to object you created called `car1`.
- A property can also be deleted as usual using the `delete` keyword or by setting the property value to empty or null. Difference is delete removed the property completely and the setting its value to empty or null will leave the property as part of the object but just removes the value it holds.
- `this` is an important keyword in JS. When a function is created at the top level of a script, it truly sits inside the `window` object as this is the top level object. This `window` object has default properties and methods available that an be used but you can access to them by prefixing them with the `this` keywoard when needing to use them. Same applies with global varibales.
- Arrays are a special type of object with automatically assigned key value assinged to each value you pass into the array. This key is the INDEX number of the array that you use to access that value.
- Keep in mind, arrays can hold objects and objects can also have array data type properites in it. The same rules to accessing the value applies but now with the dotted notation.
- JS has many built in objects and this all goes back to the saying that everying in JS is an object. You have the browser object model, document object model, global javascript. These are needed to get things going.
- The browser object model creates a model for you to access of the broswer tab or window. The window is the top most level object which them provides child objects being the document, history, location, navigation and screen. There are many more and a search online will give you the info needed.
- Global objects do not form a single model but are groups of individual objects that relate to different parts of the JS language.
- JS adds many of these object methods to the varibales and other items you create in JS automatically an example being `.toUpperCaser()` that is added to any string you create. These are all helper methods defaulted to the string data type.
- Another global object that you will use often is the `Date()`. This object has various methods that allow you to manipulate the date that you are working with.

[Return to 201 TOC](201TOC.md)

[Return to Main Page](../README.md)
