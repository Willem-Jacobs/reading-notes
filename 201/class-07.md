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

- 

[Return to 201 TOC](201TOC.md)

[Return to Main Page](../README.md)
