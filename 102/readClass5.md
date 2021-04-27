# Class 5 - CSS Basics & Color Reading

- CSS used to style your HTML for the web page.
- Can apply colors, images, font, size of font, positioning. The possibilities are endless with CSS.
- There are block elements and inline elements from HTML page and these can all be styled.
- Selection to items in the HTML page can be done in various ways:
  - Element name example of `<div>, <section>, <h1>`, etc.
  - Class name. The class name you assign to the element in HTML.
  - ID name. The ID name assigned to an element.
  - Child selector.
  - Descendant selector.
  - Adjacent sibling selector.
  - General sibling selector.
  - `*` selects everything for all elements. This used when you want to set a global setting to ALL elements. Usually placed at the top of the CSS file.
- Values are assigned using a property name and a value assigned to that property.
- CSS is best to use an external file with all the CSS. There an be multiple files but the load order is important as the last element being set is the rule used overriding any previous settings. This is called the cascading effect. This is set using the HTML `<link>` element along with setting a `href, type, rel`.
- Inline style can also be set directly to the HTML but this not good to use. Use the `<style>` tag for setting inline values.

## Color

- Colors using various methods to set. These are
  - RGB
  - HEX value
  - Defined name
- Ensure to use colors that blend well together providing a good contrast.
- Opacity can also be set using the RGBA color setting.
- CSS3 added HSL and HSLA for color choice setting. HSL lets you add HUE, Saturation and Lightness. HSLA adds a 4th property to add transparency.
- 

[Return to 102 TOC](102toc.md)

[Return to Main Page](../README.md)