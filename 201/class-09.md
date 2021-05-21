# HTML/JavaScript Book Reading

[Return to 201 TOC](201TOC.md)

## Chapter 7 - Forms (pp.144-175)

*Resource: Duckett HTML Book* - Various parts cited from the resource

- Forms provide a set of elements to collect data from your users.
- Form elements include: Text input, password input, text area (multi-line). For making choices you have: radio buttons, checkboces and drop-down boxes. For submitting the form you have: submit button, image button and upload. Others also exist.
- Forms work by gathering the data and submitting it to a server to process to save, act upon and returns other data or a message.
- The back-end needs to know the pairing of the data so a name/value or key pair is used to send the data to the server either in the URL or in the HTTP header.
- All forms start with an element of `<form> </form>` with the rest of the elements between the open/close tags. The form has an attribute of action and ID that need to be set. An optional attribute is `method="get" or "post"` and defaults to `get`. The ID is used to identify the form from others and used by scripts.
- Input element `<input> />` needs serveral attributes that are required set: type, name. The name is used with the name/value (key pair). Maxlength is another attribute that can be used to provide a max length value.
- The type attribute for the input field can have values of "text", "password", "radio", "checkbox", "file", "submit", "image", "hidden", "date", "email, "url", "search".
- Text area `<textarea> </textarea>` is used for multi-line text input fields. Default text between the `><` will appear in the box when first load to provide a message to the user of what to enter. The browser will send this text to the servier if not deleted so use with caution.
- A radio button uses the `<input> />` with type set to "radio" and the following attributes need to be set: name, value, checked, action. Name is used for the name/value pair, value is used for the text to display next to the radio button, checked is used if this option is defaulted to checked (selected). Only 1 radio button in a group can be seleted.
- A checkbox uses the `<input> />` with type set to "checkbox". This uses the same attributes as a radio button of name, value, checked. The value indicates the value that is send to the back-end along with what is shown on the form next to the checkbox. A checkbox can be checked or unchecked. Values can be 1 or more of the group and can be on/off.
- Dropdown box uses the `<select> </select>` element with a name attribute. Between the open/close tag you have to add the `<option> </option>` element which has a value attribute that is used for the back-end and the text to display in the dropdown list is between the `><` of the open/close of the `<option>`. A selected attribute can be set on the `<option>` with a value of "selected" to default that value as the value to display and is the default selection. If no selection is set, the first option is set as the default.
- A dropdown can be set to allow multiple selections by adding the `size` and `multiple` attributes. The size is used to set the number of choices to display from all the options and the `multiple` attribute should have `="multiple"` value which then allows the user to select more than 1 of the options. The CTRL or COMMAND key has to be held down to make multiple selections.
- An `<input> />` with the type set to `type="file"` will create an input field with a browse button next to it to allow the user to click on this button and open a window on their computer to select a file to upload. When using this, the method for the form has to be a "post".
- A submit button can be made using the `<input> />` with a `type="submit"` along with a name attribute and with a `value="some text"` for the button text.
- An iamge can also be displayed as the button by setting the `type="image"` attribute and providing the `src="image file"` and a `width & height` attribute needs to be set for the button size to display. The `alt="some value"` should also be set.
- A `<button> </button>` element can be used with all the standard default attributes for a button like image and the value to display on the button between the `><`.
- An `<input> />` with a type of "hidden" can be used to have hidden information that the form submits to the back-end. This used for default information that the user should not change or need to know about.
- A `<label></label>` element tag can be used as a wrapper around form elements to provide a label that will be displayed. This helps screen readers. If not used as a wrapper, the label can be set by setting a `for="input field ID name"` attribute on the label and this will link it to that form element. For form elements with a name, the name is specified in the `for` attribute.
- Form elements can be grouped by wrapping them inside the `<fieldset> </fieldset>` element tags with a `<legend></legend>` element tag right after to provide a name for the grouped section.
- HTML has form validation from teh browser but the book does not say much about it.
- A `type="date"` can be used on the input element to create a date like input field.
- A `type="email" or type="url"` can be set on the input form element to assist the browser with default validation that the value entered matches those types.
- A `type="search"` can be set on the form input element to default a search box with some default items added like a clear icon in the text field.
- A `placeholder="some text"` can be set on input elements to show a default value to the user that will be cleared when the user enters their information in the field.

## Chapter 14 - Lits, Tables & Forms - CSS (pp.330-357)

*Resource: Duckett HTML Book* - Various parts cited from the resource

- `list-style-type` can be applied to `<ol>, <ul>, <li>`. For unordered-lists you have values of `none, disc, circle, square` to use as the bullets that are displayed. For ordered-lists you have values of `decimal, decimal-leading-zero, lower-alpha, upper-alpha, lower-roman, upper-roman` to define the type of bullet displayed.
- Images can also be used as the bullet by using the `list-style-image: url("image filename");` property.
- `list-style-position` can be used to defile if the bullet will display on the inside or outside of the box containing the main points. The values are `outside or inside`.
- A shorthand can be used to set the above values `list-style: position type`. example: `list-style: inside circle;`.
- Tables can be provided many styling options. Width sets the width of the entire table. Padding to set the space between the border of each table cell and its content. Text-transform to convert text to other cases. letter-spacing, font-size, border-top, border-bottom, text-align, background-color and :hover can all be set.
- `empty-cells: show, hide inherit` can be set to determine if to show or hide empty cells of the table.
- `border-spacing` can be set with pixel value first number is horizontal spacing, second number is vertical spacing between adjacent cells.
- `border-collapse: collapse, seperate` can be used where collapse will merge the borders where it can be done and seperate will obey the settings from border-spacing and empty-cells.
- Forms need to be styled using standard CSS properites to group, align, box, size, etc to make the form attractiver and easy to use.

## Chapter 6 - Events (pp.243-292)

*Resource: Duckett JavaScript and Jquery Book* - Various parts cited from the resource

- Events are used to create interaction, trigger code to be ran and responds to users.
- Events are fired or are raised and events trigger scripts to be ran.
- There are various types of events that can be raised to UI events, keyboard events, mouse events, focus events, form events, mutation events.
- Events are linked to an element that are then bound to a specified event along with the function that will be raised/fired.
- There are 3 types of event handlers being: HTML Events Handlers (not used much anymore), traditional DOM event handlers but these allow only 1 function to be called so is not used much and the last is event listeners which is widely used as it can trigger multiple functions and pass values.
- Will focus on the 3rd option of event listeners as that is the more widely used type.
- `element.addEventListner('event', functionName [, boolean]);` is the format used where the value in [] is optional for the method to control the capture and is usually set to false (default value). You need to have a reference to the element first in a varibale. Event listeners are added, usually, at the end of your JS script file. Do not call the function by adding the (). You are only setting a reference to it.
- Should values need to be passed or more functions called, you use an anonymous function call by replacing the functionName with `function() {} [, boolean]);` inside the {} you call the function(s) and passing in any values needed between the ().
- Event listeners can be bound to elements, parent elements up the node, document object, window object. When you go from inside out, this is called bubbling the event which is the default option. Event capturing lets the event start from the least specific and flow inward to the most specific one. By setting the last parameter (boolean to true or false) you control the flow direction where TRUE is capturing phase and FALSE = bubbling mode (default).
- A default object normall called `event or e` is passed each time an event is raides/fired. This event object has all the data and valuable information in it you can use in your code. This event object is passed to any function that is the event handler or listener. If using an anonymous function, this function will get the event object but you have to add it between the () as event or e, your choice, and then you have to pass it on to the function being called inside the {} as the first value then your values after.
- Event delegation can be used to listen for an event on a parent element due to the use of the bubbling flow. This eliminates the need for event listeners on child elements and creating too many of them when you have a list, table or many buttons. You can use the event object to determine which element raised/fired the event. Too many listeners slows down your code and increases the usage of memory.
- Event delegation also works with new elements you add to the parent using code, solves the limitations with the `this` keyword and simplifies your code.
- preventDefault() and stopPropagation() to prevent default behaviour on forms or other redirection to a new page so you can stay on the form for validation or other reasons and stopPropagation is used to stop the bubbling up from the current element that handled the event.
- The event object target property provides the elemnt the event occured on.
- Mutation Observers provide you feedback of changes to the DOM by waiting till all changes are done and then providing the changes as a batch that you can react upon with code.
- HTML5 page-level events provide event triggers based on mutation listed above like `DOMContentLoaded, hashChanged, beforeunload`.

[Return to 201 TOC](201TOC.md)

[Return to Main Page](../README.md)

