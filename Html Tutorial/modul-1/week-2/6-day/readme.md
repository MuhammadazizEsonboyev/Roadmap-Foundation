## CSS Display

CSS Layout - The display Property

The most important CSS property for controlling layout is the  'display' property, and it states how an 

element is to be displayed. The default display value for most HTML elements is block or inline


Block-level Elements


A block-level element always starts on a new line and takes up the full width available (stretches out to 

the left and right as far as it can).
The <div> element is a block-level element.

Examples of block-level elements:

    <div>
    <h1> - <h6>
    <p>
    <form>
    <header>
    <footer>
    <section>


Inline Elements

Inline Elements

An inline element does not start on a new line and only takes up as much width as necessary.

This is an inline <span> element inside a paragraph.

Examples of inline elements:

    <span>
    <a>
    <img>


Display: none;

display: none; is commonly used with JavaScript to hide and show elements without deleting and recreating 

them. Take a look at our last example on this page if you want to know how this can be achieved.

The <script> element uses display: none; as default. 






Override The Default Display Value
To override the default display value of every element, simply change an inline element to a block element 

or vice versa. This also allows you to make the page the way you like while complying with the web 

standards. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
li {
  display: inline;
}
</style>
</head>
<body>

<p>Display a list of links as a horizontal menu:</p>

<ul>
  <li><a href="/html/default.asp" target="_blank">HTML</a></li>
  <li><a href="/css/default.asp" target="_blank">CSS</a></li>
  <li><a href="/js/default.asp" target="_blank">JavaScript</a></li>
</ul>

</body>
</html>


Note: Setting the display property of an element only changes how the element is displayed, NOT what kind of 

element it is. So, an inline element with display: block; is not allowed to have other block elements inside 

it.


To display <span> elements as block elements:


<!DOCTYPE html>
<html>
<head>
<style>
span {
  display: block;
}
</style>
</head>
<body>

<span>A display property with a value of "block" results in</span> <span>a line break between the two 

elements.</span>

</body>
</html>



The following example displays <a> elements as block elements:


<!DOCTYPE html>
<html>
<head>
<style>
a {
  display: block;
}
</style>
</head>
<body>

<p>Display links as block elements:</p>

<a href="/html/default.asp" target="_blank">HTML</a>
<a href="/css/default.asp" target="_blank">CSS</a>
<a href="/js/default.asp" target="_blank">JavaScript</a>

</body>
</html>



Hide an Element - display:none or visibility:hidden?

Setting the display property to none enables an element to be hidden and display the page as if the element 

is not there. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
h1.hidden {
  display: none;
}
</style>
</head>
<body>

<h1>This is a visible heading</h1>
<h1 class="hidden">This is a hidden heading</h1>
<p>Notice that the h1 element with display: none; does not take up any space.</p>

</body>
</html>





Setting visibility:hidden; also hides an element. However, the element will still take up the same space as 

before. The element will be hidden, but still affect the layout: 


<!DOCTYPE html>
<html>
<head>
<style>
h1.hidden {
  visibility: hidden;
}
</style>
</head>
<body>

<h1>This is a visible heading</h1>
<h1 class="hidden">This is a hidden heading</h1>
<p>Notice that the hidden heading still takes up space.</p>

</body>
</html>


Additional Examples:

The differences between display:none; and visibility:hidden; is shown in the example below. 

visibility:hidden hides the element, but it still takes up space in the layout.

display:none removes the element from the document. It does not take up any space.


<!DOCTYPE html>
<html>
<head>
<style>
.imgbox {
  float: left;
  text-align: center;
  width: 120px;
  border: 1px solid gray;
  margin: 4px;
  padding: 6px;
}

button {
  width: 100%;
}
</style>
</head>
<body>

<h3>Difference between display:none and visiblity: hidden</h3>
<p><strong>visibility:hidden</strong> hides the element, but it still takes up space in the layout.</p>
<p><strong>display:none</strong> removes the element from the document. It does not take up any space.</p>

<div class="imgbox" id="imgbox1">Box 1<br>
  <img src="img_5terre.jpg" alt="Italy" style="width:100%">
  <button onclick="removeElement()">Remove</button>
</div>

<div class="imgbox" id="imgbox2">Box 2<br>
  <img src="img_lights.jpg" alt="Lights" style="width:100%">
  <button onclick="changeVisibility()">Hide</button>
</div>

<div class="imgbox">Box 3<br>
  <img src="img_forest.jpg" alt="Forest" style="width:100%">
  <button onclick="resetElement()">Reset All</button>
</div>

<script>
function removeElement() {
  document.getElementById("imgbox1").style.display = "none";
}

function changeVisibility() {
  document.getElementById("imgbox2").style.visibility = "hidden";
}

function resetElement() {
  document.getElementById("imgbox1").style.display = "block";
  document.getElementById("imgbox2").style.visibility = "visible";
}
</script>

</body>
</html>



CSS can also be used together with Javascript to show an element on click as shown below:

CSS Display/Visibility Properties
Property 	Description
display 	Specifies how an element should be displayed
visibility 	Specifies whether or not an element should be visible

<kbd>return</kbd>[Back to table of contents](#homepage)


--------

## HTML Iframes 

It is used to display a webpage within another webpage

* HTML Iframe syntax

HTML Iframe Syntax:

```<iframe>``` tag specifies an inline frame. This inline frame is used to  embed another document within the current html document

** Syntax example below

```<iframe src="url" title="description">```

NB: It is a good practice to always include a title attribute for the <iframe>. This is used by screen readers to read out what the content of the iframe is.


** Use height and width to specify the size ofthe iframe
```
<iframe src="demo_iframe.htm" height="200" width="300" title="Iframe Example"></iframe>
```

** You can also add style attribute and use css height and width properties:
```
<iframe src="demo_iframe.htm" style="height:200px;width:300px;" title="Iframe Example"></iframe>
```
** Iframe-Remove the border

* To remove border add style attribute and use the CSS border property. 
```
<iframe src="demo_iframe.htm" style="border:none;" title="Iframe Example"></iframe>
```

* You can also use css style to change the size and color of the iframe's border:

```
<iframe src="demo_iframe.htm" style="border:2px solid red;" title="Iframe Example"></iframe>
```

Iframe - Target for a Link

An iframe can be used as the target frame for a link. The target attribute of the link must refer to the name attribute ofthe iframe
```
<iframe src="demo_iframe.htm" name="iframe_a" title="Iframe Example"></iframe>

<p><a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a></p>
```

** When the target attribute of a link matches the name of an iframe, the link will open in the iframe


In essence, the target of a url can be a new (_blank) page and  can also be the name (attribute) of an iframe

<kbd>return</kbd>[Back to table of contents](#homepage)

---------

## HTML JavaScript
Javascript inclusion in HTML makes it more interactive and dynamic.


** The below gives a button that shows date and time.
```
<!DOCTYPE html>
<html>
<body>

<h1>My First JavaScript</h1>

<button type="button"
onclick="document.getElementById('demo').innerHTML = Date()">
Click me to display Date and Time.</button>

<p id="demo"></p>

</body>
</html> 
```

* HTML Script tag.

It defines client-side JavaScript...the the <script> element contains script statement or points to an external script through an src attribute. JS is used for image manipulation, form validation, and dynamic changes of content.

To select an HTML element, JavaScript most often uses the ```document.getElementById()``` method.

This JavaScript example writes "Hello JavaScript!" into an HTML element with id="demo":
```
<h2>Use JavaScript to Change Text</h2>
<p>This example writes "Hello JavaScript!" into an HTML element with id="demo":</p>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script> 
```

** Use JavaScript to change the style of an HTML document
```
<h1>My First JavaScript</h1>

<p id="demo">JavaScript can change the style of an HTML element.</p>

<script>
function myFunction() {
  document.getElementById("demo").style.fontSize = "25px"; 
  document.getElementById("demo").style.color = "red";
  document.getElementById("demo").style.backgroundColor = "yellow";        
}
</script>

<button type="button" onclick="myFunction()">Click Me!</button>
```

** Use Javascript to change the src attribute of an image.
```document.getElementById("image").src = "picture.gif";```

* see full code below
```
<h1>My First JavaScript</h1>
<p>Here, a JavaScript changes the value of the src (source) attribute of an image.</p>

<script>
function light(sw) {
  var pic;
  if (sw == 0) {
    pic = "pic_bulboff.gif"
  } else {
    pic = "pic_bulbon.gif"
  }
  document.getElementById('myImage').src = pic;
}
</script>

<img id="myImage" src="pic_bulboff.gif" width="100" height="180">

<p>
<button type="button" onclick="light(1)">Light On</button>
<button type="button" onclick="light(0)">Light Off</button>
</p>
```

* HTML ```<noscript>``` tag

Defines alternate content to be displayed to users that have disabled scripts in their browsers or have browsers with no support for scripts

* This is the script 
```
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
<noscript>Sorry, your browser does not support JavaScript!</noscript> 

**The full script is:
<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>

<noscript>Sorry, your browser does not support JavaScript!</noscript>

<p>A browser without support for JavaScript will show the text written inside the noscript element.</p>
```
<kbd>return</kbd>[Back to table of contents](#homepage)


