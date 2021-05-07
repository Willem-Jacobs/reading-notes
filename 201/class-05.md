# HTML Book Readings

[Return to 201 TOC](201TOC.md)

*Resource: Duckett HTML Book* - Various parts cited from the resource

## Chapter 5 - Images (pp.94-125)

- Images should be stored in their own folder on your site. This folder can be broken down further into sub-folders.
- Images are added to the HTML (can also be added from the CSS file) by using the `<img src="location/filename.ext" alt="alternate text" title="some title">` The title is used as a tooltip when hovering (most browsers) and the alt is used for screen readers. The src is the source location, filename & extention of the image to display. The src and alt are required. This element is a self closing element.
- Images are best displayed (should be included for browser loading/display optimization) by adding the `height & width` attributes to the `<img>` element. The size of image can also be specified in the CSS file.
- There are 3 rules to creating/using images.
  - Save images in the right format (jpeg, gif or png).
  - Save images at the right size. (size & width needed).
  - Use the correct resolution. (Based on 72px per inch).
- JPEG should be used when you have many different colors in a picture.
- GIF or PNG when using images with few colors (flat color) or a large area of the same color. Like logos, diagrams and illustrations.
- Should save your images to the same size that you want to display them.
- Taking a small image size source and enlarging will distort the image. Best not to do this.
- Ensure when cropping an image you do not lose key information of the image.
- Image resolution has a big impact on the file size which then has an impact on downloading time to display on the page. Best to save images that are 72ppi (pixel per inch) as that all a computer display can show. Higher resolution of the image on a computer display has no benefit.
- SVG (Scalable Vector Graphics) is a new format, great options and quick. They are used heavily now but this book does not talk much about them.
- Animated GIF show several frames of an image in sequence proving a simple animation.
- PNG are best for transparent images.
- HTML5 has a `<figure></figure>` element that you use as a wrapper around the `<img />` and include a `<figcaption></figcaption>` element inside. More than 1 image can be inside the figure element as long as they all share the image caption.

## Chapter 11 - Color (pp.246-263)

- To set the color of text use the `color` property. This can take a color name, hex value, RGB, RGBA, HSL, HSLA. The values that end with "A" can take an Alpha value for opacity.
- To set the background color use the `background-color` property and this can take the same values as the color property.
- RGB uses 3 values that are numbers from 0-255 that specify red, green and blue. HSL take hue, saturation and lightness. Hue is a degree on the color wheel from 0-360. 0 (or 360) is red, 120 is green, 240 is blue. Saturation is a percentage value 0% means a shade of gray and 100% is the full color of gray. Lightness is also a percentage 0% is black while 100% is white.
- The alpa channel is a value between 0.0 to 1.0 with 0 being fully transparent and 1 being fully opaque.
- When picking a foreground and a background color, keep in mind the contrast to ensure that there is enough contract for the text to be legible.
- There is an `opacity` property that can be used that takes a number from 0.0 to 1.0 with 0.0 is fully transparent and 1.0 being fully opaque.

## Chapter 12 - Text (pp.264-299)

- Browsers main fonts are a serif font, sand-serif font or monospace. These are installed on all machines but there is some customization the end user can do to the browser.
- There are weights of light, medium, bold and black.
- There are styles of normal, italic and oblique.
- There are stretch of condensed, regular and extended.
- Selection of a font is done with the font-family setting in CSS where you can specify a main font and a few backup options. You can specify a direct font name or use the defaults of serif, sans-serif and monospace. If the font name is 2 words, enclose it in quotes. `font-family: font name, backup font, backup font`
- The size of the letters can be specified using the `font-size:` property. The value can be specified in pixel with `px` or percentage of the base size of 16px. Can also specify with em or rem where 1em or 1rem is the default of 16px.
- In CSS you can import other fonts from local drive or from websites by using the `@font-face {}` property where inside the {} you specify the font-family and the src of the location to import from.
- There are various font formats with the most supported and used being SVG.
- The weight of the text can be changed using the `font-weight:` property with values of normal, bold, light, medium and black.
- The font style can be changed with the `font-style:` property values of italic, normal or oblique.
- The case of text can be changed by using the `text-transform:` property and the values of uppercase, lowercase or capitalize.
- You can apply `text-decoration:` by providing values of none, underline, overline, line-through or blink.
- The spacing between lines can be adjusted by using the `line-height:` property. This the same as line spacing in a word processor. A value of pixel, em or rem can be used.
- Letter spacing and word spacing can also be specified using the `letter-spacing: and word-spacing` properties. This good for headline text but not in normal text as it can make reading harder.
- Alignment can be adjusted by using the `text-align:` property with the values of left, right, center or justify.
- Vertical alignment can also be used with the `vertical-align:` property passing in a value of baseline, sub, super, top, text-top, middle, bottom or text bottom. One key point to remember is this does not align the text in a block level element. It is commonly used with inline elements.
- The first line of a text block can be indented by using the `text-indent:` property and passing in a number value of pixel, em or rem.
- Similar to box shadow, you can also set text-shadow by using the `text-shadow:` property. The values passed in are the same as using `box-shadow`.
- You can use a psuedo-element of `:first-letter` to change the look of the first letter of a word or use the `:first-line` to change the look of the entire line. These are used after the selector example being `p.into:first-letter` as the selector and inside the {} you can specify different property/parameter setting you want to use.
- Other psuedo-elemnts that can be used are `:link, :visited, :hover, :active, :focus` to use on links, buttons, list elements in menus etc. The order is important and need to be used in the order shown.

## Blog Post - [JPEG vs PNG vs GIF](https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d)

[Return to 201 TOC](201TOC.md)

[Reutrn to Main Page](../README.md)
