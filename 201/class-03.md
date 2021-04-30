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

[Return to 201 TOC](201TOC.md)

[Reutrn to Main Page](../README.md)
