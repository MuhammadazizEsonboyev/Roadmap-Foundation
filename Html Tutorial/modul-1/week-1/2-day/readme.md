## HTML ATTRIBUTES
 **Attribute comes as name="value"
* HTML links: ```<a href="https://www.w3schools.com">Visit W3Schools</a>``` 
The SRC attribute: 
```
<h2>The src Attribute</h2>
<p>HTML images are defined with the img tag, and the filename of the image source is specified in the src attribute:</p>
<img src="img_girl.jpg" width="500" height="600">
```
**specifying the url in the ```src``` attribute
Absolute url: links to image on another site: src="https://www.w3schools.com/images/img_girl.jpg"
Relative url: Links to image hosted within the website. No domain name included here. src="img_girl.jpg"
src="/images/img_girl.jpg"   **in this case, the slash is relative to the site url
**Width and height attribute(pixels) with  ```<img>```
```
 <img src="img_girl.jpg" width="500" height="600"> 
```
**Alt attribute includes alternative text for the image incase a user can not read the image: <img src="img_girl.jpg" alt="Girl with a jacket"> 
**style attribute adds style elements like color, font, size, etc to an image
```
 <p style="color:red;">This is a red paragraph.</p> 
```
**Lang attribute: Should always be included inside an <html> tag the declare website language to assist search engines locate you
```
<!DOCTYPE html>
<html lang="en">
<body>
...
</body>
</html>
```
*You can also include country attribute.
```
<!DOCTYPE html>
<html lang="en-US">
<body>
...
</body>
</html>
```
**The title attribute: Gives extra information about an element and the attribute
will be displayed as a tooltip when mouse pointer runs over it.
```
 <p title="I'm a tooltip">This is a paragraph.</p> 
```
W3C Recommends having attributes in quote and in cases where there is a space in the attribute, you have to have the space.
*when  attribute value contains one of the quotes, use the other quote
```
<p title='John "ShotGun" Nelson'>
```
Or vice versa:
```
<p title="John 'ShotGun' Nelson"> 
```
***Attributes Summary
* All HTML elements can have attributes
* The href attribute of ```<a>``` specifies the URL of the page the link goes to
* The src attribute of ```<img>``` specifies the path to the image to be displayed
* The width and height attributes of ```<img>``` provide size information for images
* The alt attribute of ```<img>```provides an alternate text for an image
* The style attribute is used to add styles to an element, such as color, font, size, and more
* The lang attribute of the ```<html>``` tag declares the language of the Web page
* The title attribute defines some extra information about an element
<kbd>return</kbd>[Back to table of contents](#homepage)

---------------------------------------


## References
---
* [HTML forms Guide \| MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms)
* [The native form widgets](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/The_native_form_widgets)
* [HTML5 forms introduction and new attributes](http://html5doctor.com/html5-forms-introduction-and-new-attributes/)
* [HTML Form \| W3C](https://www.w3.org/TR/html5/forms.html)
* Mobile Inputs
  * [mobile input types](http://mobileinputtypes.com/)
  * [HTML5 for the mobile web – forms and input types](https://mobiforge.com/design-development/html5-mobile-web-forms-and-input-types)
* Elements: [`<form>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form),
  [`<input>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input),
  [`<label>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label),
  `<button>`, `<datalist>`, `<legend>`, `<label>`, `<select>`, `<optgroup>`, `<option>`, `<textarea>`, `<keygen>`, `<fieldset>`, `<output>`, `<progress>`
* Attributes
  * [`<form>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form#Attributes): `action`, `method`
  * [`<input>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#Attributes): `type`
  * [`<label>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label#Attributes): `for`

---------------------------------------



## HTML HEADINGS
Headings go from ```<h1> to <h6>```. Search engines use them to understand the structure of the webpage
Use h1 for main headings followed by h2 and so on
Each heading has its default size. You can change that by specifying inside a style element.
*Change your style like this:
```
<h1 style="font-size:60px;">Heading 1</h1>
```
<kbd>return</kbd>[Back to table of contents](#homepage)

---------------------------------------

## HTML PARAGRAPHS
In html, you cannot be sure of how html will be displayed on each screen size. Adding extra lines or spaces to the document does not add new lines to the page. 
Browser removes extra spaces once page displays
```
<p>This is a paragraph</p>
```
* Horizontal rules: ```<hr>``` Used to separate content(define change) and defines a thematic break in an HTML page. It shows up as an horizontal line. 
```<hr>``` tag has no closing tag since it is an empty tag.
* Line breaks: ```<br>``` element
Use this when you want a line break without starting a new paragraph.
The Poem Problem: Poems have to be included in the ```<pre>``` preformatted text tag
The ```<pre>``` tag displays text in fixed-width font (usually Courier), and it preserves both spaces and line breaks.
Tags summary
```
<p> 	Defines a paragraph
<hr> 	Defines a thematic change in the content
<br> 	Inserts a single line break
<pre> 	Defines pre-formatted text
```
<kbd>return</kbd>[Back to table of contents](#homepage)

---------------------------
## HTML STYLES
The HTML Style attribute syntax:
```
<tagname style="property:value;">
```
* Where The property is a CSS property and value is a CSS value.
* Background color: Defines the background color for an HTML element
```
<body style="background-color:powderblue;">
```
* Set background color for two different elements:
```
<h1 style="background-color:powderblue;">This is a heading</h1>
<p style="background-color:tomato;">This is a paragraph.</p>
```
**Text color
```
 <h1 style="color:blue;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p> 
```
**Fonts
```
 <h1 style="font-family:verdana;">This is a heading</h1>
<p style="font-family:courier;">This is a paragraph.</p> 
```
**Text Size
```
 <h1 style="font-size:300%;">This is a heading</h1>
<p style="font-size:160%;">This is a paragraph.</p> 
```
**Text alignment
```
 <h1 style="text-align:center;">Centered Heading</h1>
<p style="text-align:center;">Centered paragraph.</p> 
```
Styles summary
* Use the style attribute for styling HTML elements
* Use background-color for background color
* Use color for text colors
* Use font-family for text fonts
* Use font-size for text sizes
* Use text-align for text alignment
<kbd>return</kbd>[Back to table of contents](#homepage)

