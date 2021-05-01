# HTML Book Readings

[Return to 201 TOC](201TOC.md)

*Resource: Duckett HTML Book* - Various parts cited from the resource

## Chapter 3 - Lists (pp.62-73)

- HTML provides 3 types of listing options these are:
  - Ordered Lists which are indented with default of each line being numbered starting with 1.
  - Unordered Lists which are indentedd with default of each line having a bullet point.
  - Definition Lists where you have a term along with a definition. Each formated correclty with indention.
- Each type of list can be customized using CSS.
- Lists can be nested.
- Syntax for ordered and ordered lists start with open/closing tag of `<ol></ol>` then inside these tages you have the `<li></li>`. For unordered list you use the open/closing tag of `<ul></ul>` with the same `<li></li>` inside the tags.
- Definition lists syntax has outside open/close tag of `<dl></dl>` then the term being has the `<dt></dt>` and then `<dd></dd>` for the definition.

## Chapter 13 - Boxes (pp.300-320)

- CSS treats most HTML elements as it lives in its own box. This has some great benefits for styling and layout.
- You can control the dimensions of the boxes.
- You can create borders around the box, add padding and margins and hide/show the boxes with their content inside.
- Boxes can be inside other boxes.
- Dimensions of the box can be controlled with `width and height` properties. These take a value of pixel or rem or em or percentage.
- The heigh and width can be limited by using the `min-wdith, max-width, min-height, max-height` properties.
- For an item inside the box that is too big to be displayed can be controleld with `overflow` property which will hide what is not fit in the box. The `scroll` property can be used to make the content in the box scrollable.
- Each box has the content inside and around that content, you can add the property `padding` to add some space around the content. On the outside of this padding, you can add the property of `boarder` and around the border you can add the property `margin`. Each of these adds spacing in its own respective manor. This useful to add seperation between elements.
- A border stype can be applied to the box by using the `border-style` property and its values. Border style can also be applied differently to each size of the box (top, right, bottom, left).
- A border color can be applied to the box by using the `border-color` property and then specifying a color. You can also apply different colors by tageting the exact border you want. These are Top, Right, Bottom and left using `border-?????-color` where ????? is the side.
- a short hand can be used where you use `border: size style color;` where you replace size with a pixel, rem or em amount, style replaced with a style (solid, dotted, dashed, groove, ridge, inset, outset, hidden/none).
- Padding is applied by using the `padding` property then you specify a pixel, rem, em or percentage. You can apply different padding to each side by specifying top, right, bottom or right. A short hand can also be used where you specify only 2 values `padding: 5px 10px` which would apply 5px to top & bottom and 10px to left & right. If you only specify 1 value, it would be applied to all 4 sides.
- Margin is done the same way as above like padding but using the property of `margin`.
- The box you are working with can be centered by setting `left-margin and right-margin` to auto but the width of the box must be set. By doing this, the box will auto center with equal spacing on each side of the box. Note that if the box is within another element, it will center within that element.
- `display` lets you change the an in-line element into a block-level element or vice versa. It is also used to hide an element from the page. You have a few values here being `inline, block, inline-block, none`.
- `visibility` allows you to hide boxes but still leaves a the space visible where the element would have been. The values for this are `hidden & visible`.
- The box item can also have a shadow by using the `box-shadow` property. You set a horizontal offset, vertical offset, blur distance and spread of shadow. Positive and negative numbers can be used to change the location of the shadow. 2 of these values are required being the horizontal and vertical offset and a color example `box-shadow: 5px 5px 5px black`. You can add the inset keywoard before any values to have the shadow on the inside of the box.
- `border-radius` is used to set the radius of the corners of the box. This will give you rounded corners. Higher value would be a larger rounded corner. You normally just provide a single value but you can specify for the top-right, bottom-rigt, top-left, bottom-left by inserting the text between border & radius. A short hand can be used by specifying `border-radius: 10px, 15px, 10px, 15px` isntead of typing the entire commands for each corer.

## Chapter 4 - From Switch Statements to end (pp.162-182)

*Resource: Duckett JS Book* - Various parts cited from the resource.

- A switch statement can be used instead of if..else if many cases and you gain a better performance. The swithc statments checks for a certain conidtion, usually this is a variable. Then you have a case check for the possible values of the variable and if this matches, the code in that case is ran. You use the break keyword to exit the switch after the code block runs to continue execution after the entire switch. One benefit of the switch statement is the ability to provide a default code block to run should none of the values match a case statement.
- JS us a weak type language thus it will try to convert certain data types for you and this is called **type coercion** and should be avoided at all costs. You should always use strict operators `=== or !==` instead of the operators that do not check for data type.
- JS with its type coercion can treat every value as if it were true or false. Example a 0 is false and a 1 is true (similar to binary with a 0 is off and a 1 is on). If a variable has a value it would be true (thuthy).
- Short Circuit is a way of JS exits conditional checks as soon as a true value is found. This means that the remaining coditions would not be checked. This very useful in the code.
- Loops are used for many purposes in the code. There are 3 loop types for JS. The `for` the `while` and the `do while`
- The keywords of `break` and `continue` are used often with loops. Break to exit the loop and continue with the current iteration and check the condition again.
- For loop is the most used. The while loop you have to increase the counter value yourself for each iterations and the code could have the ability to not even run. The do while loop does the condition check at the end of the code block so the code block will always run once.

[Return to 201 TOC](201TOC.md)

[Reutrn to Main Page](../README.md)
