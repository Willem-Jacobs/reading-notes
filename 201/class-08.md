# HTML/JavaScript Book Reading

[Return to 201 TOC](201TOC.md)

## Chapter 15 - Layout (pp.358-404)

*Resource: Duckett HTML Book* - Various parts cited from the resource

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

[Return to 201 TOC](201TOC.md)

[Return to Main Page](../README.md)
