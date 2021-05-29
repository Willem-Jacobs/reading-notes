# HTML/JavaScript Book Reading

[Return to 201 TOC](201TOC.md)

## Chapter 16 - Images (pp.406-427)

*Resource: Duckett HTML Book* - Various parts cited from the resource

- Images use the `width & height` settings and is best to set this in CSS. This helps the page to load faster by telling the browser how much space to leave for the image and keeps rendering the page.
- Setting common image sizes is best practice in CSS to define small, medium and large as img classes and then set this class in the HTML.
- Best pratice to make another class for alignment using the float and other margin/padding settings and assign this class to the HTML element along with the size class.
- To center an image, need to change it to a block level element then use the standard method used to center block elements by setting margin to auto.
- An image can be used to set an image as the background to any HTML element. Use the `background-image: url("file path/name")`. You can repeat the iamge in the element, if needed, by setting the `background-repeat:` property with the values of `repeat, repeat-x, repeat-y, no-repeat`.
- Using the `background-attachment:` property can be set to control if the image remains fixed or will scroll as the user scrolls up/down the page. Values are `fixed, scroll`.
- The `background-position:` property can be used to specify where in the browser the image will be blaced as long as the image is not repeating. The values are usualy specified as pairs but if only the first value is used, the second value is always `center`. The values are: `left top, left, center, left bottom, center top, center center, center bottom, right top, right center, right bottom`. Pixel or percentage values can also be used as the pair values and then this will start from the top left corner. The value pairs are 1st = horizontal, 2nd = vertical.
- A shorthand can be used for all of the above but the order does matter. `background:` is the short hand and the values need to be in the order of: color, image, repeat, attachment, position. You can skip a value if it is not needed to be set.
- Image rollovers & sprites can be set for elements using CSS. This monitors the hover and active psuedo classes. In the CSS just different states are created for the desired outcome. This is done by moving the position of an image.
- Image background contrast can be set to allow text to overlay the image or use a semi-transparent background color for your text element.

## Chapter 19 - Practical Information (pp.476-492)

*Resource: Duckett HTML Book* - Various parts cited from the resource

- Search Engine Optimization (SEO) is settings in your page of keywords that are used by search engine crawlers to get info on your page.
- The SEO settins for your page are split into 2 parts. On-Page and Off-Page.
- On-Page has 7 key areas for information to be placed as the crawler looks over your HTML page.
- Off-Page relates to how other sites link to your page and crawlers will look at your page's links in the `<a>` tags.
- On-Page use keywoards in the Title, URL/web address, headings, text, link text, image alt text and info in the `<head>` section with the element of `<meta>`.
- Analytics is all about learing about your visitors by tracking visits, unique visits, page views, pages per visor, average time on site and many more values. This is done using a 3rd party service.
- Hosting your site requries a hosting service, domain name and transfering the site to this service using FTP packages.

## MDN article on audio and video elements

*Resource: <https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs>

- HTML has good video/audio options.
- Controls has to be specified to get the controls visible for the video/audio.
- Controls can customized using HTML, CSS & JS along with the browser API.

[Return to 201 TOC](201TOC.md)

[Return to Main Page](../README.md)

