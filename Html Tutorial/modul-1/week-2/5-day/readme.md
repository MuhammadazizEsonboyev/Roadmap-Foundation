## HTML CLASSES

** html class attribute is used to specify a class for an html element. 

* Multiple html elements can also share the same class.
* Class attribute is used to point to a class to manipulate together in a style sheet. Javascript can also manipulate elements in the same class together.

** In the example below, all three div elements with class city are style equally together equally according to the .city style definition in the header.
```
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  border: 2px solid black;
  margin: 20px;
  padding: 20px;
}
</style>
</head>
<body>

<div class="city">
  <h2>London</h2>
  <p>London is the capital of England.</p>
</div>

<div class="city">
  <h2>Paris</h2>
  <p>Paris is the capital of France.</p>
</div>

<div class="city">
  <h2>Tokyo</h2>
  <p>Tokyo is the capital of Japan.</p>
</div>

</body>
</html> 
```



** Here we can also style note class in ```<span>``` elements with .note style definition

```
<!DOCTYPE html>
<html>
<head>
<style>
.note {
  font-size: 120%;
  color: red;
}
</style>
</head>
<body>

<h1>My <span class="note">Important</span> Heading</h1>
<p>This is some <span class="note">important</span> text.</p>

</body>
</html> 
```
NB

Tip: The class attribute can be used on any HTML element.

Note: The class name is case sensitive!


* The Syntax for Class. 

To create a class; write a period (.) character, followed by a class name. Then, define the CSS properties within curly braces {}

```
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
}
</style>
</head>
<body>

<h2 class="city">London</h2>
<p>London is the capital of England.</p>

<h2 class="city">Paris</h2>
<p>Paris is the capital of France.</p>

<h2 class="city">Tokyo</h2>
<p>Tokyo is the capital of Japan.</p>

</body>
</html>
```
* Multiple classes. 

HTML elements can belong to multiple classes. Define multiple classes by separating the class names with a space. The element will be styled according to all classes specified. 

Below, ```<h2>``` elements belongs to both city class and also main class(```<div class="city main">```)

Below, h2 element belongs to both city class and also to the main class and will get CSS styles from both of the classes
```
<h2 class="city main">London</h2>
<h2 class="city">Paris</h2>
<h2 class="city">Tokyo</h2>
```

* The full html
```
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
} 

.main {
  text-align: center;
}
</style>
</head>
<body>

<h2>Multiple Classes</h2>
<p>Here, all three h2 elements belongs to the "city" class. In addition, London also belongs to the "main" class, which center-aligns the text.</p>

<h2 class="city main">London</h2>
<h2 class="city">Paris</h2>
<h2 class="city">Tokyo</h2>

</body>
</html>
```

Different HTML elements like ```<p>``` and ```<h2>``` points to city class ans share same style
	
```
<h2 class="city">Paris</h2>
<p class="city">Paris is the capital of France</p>
```
** Use ofthe class Attribute in Javascript
Class name can also be used by JS to perform certain tasks for specific elements. 
JS usually access elemetns with a specific class name with the ```getElementByClassName()``` method:

```
<script>
function myFunction() {
  var x = document.getElementsByClassName("city");
  for (var i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
}
</script> 
```
<kbd>return</kbd>[Back to table of contents](#homepage)


---------


## HTML ID
HTML ID ATTRIBUTE: Used to specify a unique id for an HTML element.

Only one element has a particular id. 


The id attribute is used to point to a specific style declaration in a style sheet. Also used by JS to access and manipulate elements with the specific id. 

id syntax: write hash ```(#)``` followed by an id name. Then define the CSS properties with curly braces {}. in the sheet below, ```<h1>``` element is styled according to the 
HashmyHeader style definition in the header section

```
<!DOCTYPE html>
<html>
<head>
<style>
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}
</style>
</head>
<body>

<h1 id="myHeader">My Header</h1>

</body>
</html> 
```

** The id name is case sensitive! And it must contain at least one character, and must not contain whitespaces (spaces, tabs, etc.).

Diff between Class and ID: Class can be used by multiple HTML elements while id name must only be used by one HTML element within the page. 

** Below we illlustrate the difference between Class and ID
```
<!DOCTYPE html>
<html>
<head>
<style>
/* Style the element with the id "myHeader" */
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}

/* Style all elements with the class name "city" */
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
} 
</style>
</head>
<body>

<h2>Difference Between Class and ID</h2>
<p>A class name can be used by multiple HTML elements, while an id name must only be used by one HTML element within the page:</p>

<!-- An element with a unique id -->
<h1 id="myHeader">My Cities</h1>

<!-- Multiple elements with same class -->
<h2 class="city">London</h2>
<p>London is the capital of England.</p>

<h2 class="city">Paris</h2>
<p>Paris is the capital of France.</p>

<h2 class="city">Tokyo</h2>
<p>Tokyo is the capital of Japan.</p>

</body>
</html>
```

** HTML Bookmarks with ID and Links. 

Html bookmarks allows readers to jump to a specific part of a webpage, useful for very long pages. 

To use a bookmark, create it and then add a link to it. Once link is clicked, page scrolls to the location with the bookmark.


** To create a bookmark, 

```<h2 id="C4">Chapter 4</h2>```


* To add a link to it:
```
<a href="#C4">Jump to Chapter 4</a> 
```
* To add a link to the bookmark (Jump to Chapter 4) from another page.

```
<a href="html_demo.html#C4">Jump to Chapter 4</a>
```

** See the demonstration below:
```
<!DOCTYPE html>
<html>
<body>

<p><a href="#C4">Jump to Chapter 4</a></p>
<p><a href="#C10">Jump to Chapter 10</a></p>

<h2>Chapter 1</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 2</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 3</h2>
<p>This chapter explains ba bla bla</p>

<h2 id="C4">Chapter 4</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 5</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 6</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 7</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 8</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 9</h2>
<p>This chapter explains ba bla bla</p>

<h2 id="C10">Chapter 10</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 11</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 12</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 13</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 14</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 15</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 16</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 17</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 18</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 19</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 20</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 21</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 22</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 23</h2>
<p>This chapter explains ba bla bla</p>

</body>
</html>
```

* Using the id Attribute in JavaScript

The id attribute can also be used by JavaScript to perform some tasks for that specific element.

JavaScript can access an element with a specific id with the ```getElementById()``` method:

```
<script>
function displayResult() {
  document.getElementById("myHeader").innerHTML = "Have a nice day!";
}
</script> 
```

* Chapter Summary::
Chapter Summary
The id attribute is used to specify a unique id for an HTML element
The value of the id attribute must be unique within the HTML document
The id attribute is used by CSS and JavaScript to style/select a specific element
The value of the id attribute is case sensitive
The id attribute is also used to create HTML bookmarks
JavaScript can access an element with a specific id with the getElementById() method

<kbd>return</kbd>[Back to table of contents](#homepage)


-------


#CSS Backgrounds

CSS Multiple Backgrounds

In this chapter you will learn how to add multiple background images to one element.

You will also learn about the following properties:

    background-size
    background-origin
    background-clip

CSS Multiple Backgrounds

CSS allows you to add multiple background images for an element, through the background-image property.

The different background images are separated by commas, and the images are stacked on top of each other, 

where the first image is closest to the viewer.

The following example has two background images, the first image is a flower (aligned to the bottom and 

right) and the second image is a paper background (aligned to the top-left corner):


<!DOCTYPE html>
<html>
<head>
<style> 
#example1 {
  background-image: url(img_flwr.gif), url(paper.gif);
  background-position: right bottom, left top;
  background-repeat: no-repeat, repeat;
  padding: 15px;
}
</style>
</head>
<body>

<h1>Multiple Backgrounds</h1>
<p>The following div element has two background images:</p>

<div id="example1">
  <h1>Lorem Ipsum Dolor</h1>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>




Multiple background images can be specified using either the individual background properties (as above) or 

the background shorthand property.

The following example uses the background shorthand property (same result as example above):

<!DOCTYPE html>
<html>
<head>
<style> 
#example1 {
  background: url(img_flwr.gif) right bottom no-repeat, url(paper.gif) left top repeat;
  padding: 15px;
}
</style>
</head>
<body>

<div id="example1">
  <h1>Lorem Ipsum Dolor</h1>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>




CSS Background Size

The CSS background-size property allows you to specify the size of background images.

The size can be specified in lengths, percentages, or by using one of the two keywords: contain or cover.

The following example resizes a background image to much smaller than the original image (using pixels). See 

the code below:


<!DOCTYPE html>
<html>
<head>
<style>
#example1 {
  border: 1px solid black;
  background: url(img_flwr.gif);
  background-size: 100px 80px;
  background-repeat: no-repeat;
  padding: 15px;
}

#example2 {
  border: 1px solid black;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  padding: 15px;
}
</style>
</head>
<body>

<h1>The background-size Property</h1>

<p>Resized background-image:</p>
<div id="example1">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

<p>Original size of the background-image:</p>
<div id="example2">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>




The two other possible values for background-size are contain and cover.

The contain keyword scales the background image to be as large as possible (but both its width and its 

height must fit inside the content area). As such, depending on the proportions of the background image and 

the background positioning area, there may be some areas of the background which are not covered by the 

background image.

The cover keyword scales the background image so that the content area is completely covered by the 

background image (both its width and height are equal to or exceed the content area). As such, some parts of 

the background image may not be visible in the background positioning area.

The following example illustrates the use of contain and cover:

<!DOCTYPE html>
<html>
<head>
<style>
.div1 {
  border: 1px solid black;
  height: 120px;
  width: 150px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  background-size: contain;
}

.div2 {
  border: 1px solid black;
  height: 120px;
  width: 150px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  background-size: cover;
}

.div3 {
  border: 1px solid black;
  height: 120px;
  width: 150px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
}
</style>
</head>
<body>

<h1>The background-size Property</h1>

<h2>background-size: contain:</h2>
<div class="div1">
<p>Lorem ipsum dolor sit amet.</p>
</div>

<h2>background-size: cover:</h2>
<div class="div2">
<p>Lorem ipsum dolor sit amet.</p>
</div>

<h2>No background-size defined:</h2>
<div class="div3">
<p>Lorem ipsum dolor sit amet.</p>
</div>

<p>Original image:</p>
<img src="img_flwr.gif" alt="Flowers" width="224" height="162">

</body>
</html>




Define Sizes of Multiple Background Images

The background-size property also accepts multiple values for background size (using a comma-separated 

list), when working with multiple backgrounds.

The following example has three background images specified, with different background-size value for each 

image:



<!DOCTYPE html>
<html>
<head>
<style> 
#example1 {
  background: url(img_tree.gif) left top no-repeat, url(img_flwr.gif) right bottom no-repeat, url(paper.gif) 

left top repeat;
  padding: 15px;
  background-size: 50px, 130px, auto;
}
</style>
</head>
<body>

<div id="example1">
  <h1>Lorem Ipsum Dolor</h1>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>





Full Size Background Image

Now we want to have a background image on a website that covers the entire browser window at all times.

The requirements are as follows:

    Fill the entire page with the image (no white space)
    Scale image as needed
    Center image on page
    Do not cause scrollbars

The following example shows how to do it; Use the <html> element (the <html> element is always at least the 

height of the browser window). Then set a fixed and centered background on it. Then adjust its size with the 

background-size property:



<!DOCTYPE html>
<html>
<head>
<style> 
html { 
  background: url(img_man.jpg) no-repeat center fixed; 
  background-size: cover;
}

body { 
  color: white; 
}
</style>
</head>
<body>

<h1>Full Page Background Image</h1>
<p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation 

ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>

</body>
</html>



Hero Image

You could also use different background properties on a <div> to create a hero image (a large image with 

text), and place it where you want.


<!DOCTYPE html>
<html>
<head>
<style> 
html { 
  background: url(img_man.jpg) no-repeat center fixed; 
  background-size: cover;
}

body { 
  color: white; 
}
</style>
</head>
<body>

<h1>Full Page Background Image</h1>
<p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation 

ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>

</body>
</html>




The CSS background-origin property specifies where the background image is positioned.

The property takes three different values:

    border-box - the background image starts from the upper left corner of the border
    padding-box - (default) the background image starts from the upper left corner of the padding edge
    content-box - the background image starts from the upper left corner of the content

The following example illustrates the background-origin property:

<!DOCTYPE html>
<html>
<head>
<style>
#example1 {
  border: 10px solid black;
  padding: 35px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
}

#example2 {
  border: 10px solid black;
  padding: 35px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  background-origin: border-box;
}

#example3 {
  border: 10px solid black;
  padding: 35px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  background-origin: content-box;
}
</style>
</head>
<body>

<h1>The background-origin Property</h1>

<p>No background-origin (padding-box is default):</p>
<div id="example1">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

<p>background-origin: border-box:</p>
<div id="example2">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

<p>background-origin: content-box:</p>
<div id="example3">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>

  

CSS background-clip Property

The CSS background-clip property specifies the painting area of the background.

The property takes three different values:

    border-box - (default) the background is painted to the outside edge of the border
    padding-box - the background is painted to the outside edge of the padding
    content-box - the background is painted within the content box

The following example illustrates the background-clip property:

<!DOCTYPE html>
<html>
<head>
<style>
#example1 {
  border: 10px dotted black;
  padding: 35px;
  background: yellow;
}

#example2 {
  border: 10px dotted black;
  padding: 35px;
  background: yellow;
  background-clip: padding-box;
}

#example3 {
  border: 10px dotted black;
  padding: 35px;
  background: yellow;
  background-clip: content-box;
}
</style>
</head>
<body>

<h1>The background-clip Property</h1>

<p>No background-clip (border-box is default):</p>
<div id="example1">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
</div>

<p>background-clip: padding-box:</p>
<div id="example2">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
</div>

<p>background-clip: content-box:</p>
<div id="example3">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
</div>

</body>
</html>




CSS Advanced Background Properties
Property 	Description
background 	A shorthand property for setting all the background properties in one declaration
background-clip 	Specifies the painting area of the background
background-image 	Specifies one or more background images for an element
background-origin 	Specifies where the background image(s) is/are positioned
background-size 	Specifies the size of the background image(s)


<kbd>return</kbd>[Back to table of contents](#homepage)
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -   
  
 
## CSS Colors


RGBA Colors

RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity 

for a color.

An RGBA color value is specified with: rgba(red, green, blue, alpha). The alpha parameter is a number 

between 0.0 (fully transparent) and 1.0 (fully opaque). See the example below for the definition of RGBA 

colors:


<!DOCTYPE html>
<html>
<head>
<style>
#p1 {background-color:rgba(255,0,0,0.3);}
#p2 {background-color:rgba(0,255,0,0.3);}
#p3 {background-color:rgba(0,0,255,0.3);}
#p4 {background-color:rgba(192,192,192,0.3);}
#p5 {background-color:rgba(255,255,0,0.3);}
#p6 {background-color:rgba(255,0,255,0.3);}
</style>
</head>
<body>

<h1>Define Colors With RGBA Values</h1>

<p id="p1">Red</p>
<p id="p2">Green</p>
<p id="p3">Blue</p>
<p id="p4">Grey</p>
<p id="p5">Yellow</p>
<p id="p6">Cerise</p>

</body>
</html>



HSL Colors

HSL stands for Hue, Saturation and Lightness.

An HSL color value is specified with: hsl(hue, saturation, lightness).

    Hue is a degree on the color wheel (from 0 to 360):
        0 (or 360) is red
        120 is green
        240 is blue
    Saturation is a percentage value: 100% is the full color.
    Lightness is also a percentage; 0% is dark (black) and 100% is white.
The example below shows the definition of HSL colors:


<!DOCTYPE html>
<html>
<head>
<style>
#p1 {background-color:hsl(120,100%,50%);}
#p2 {background-color:hsl(120,100%,75%);}
#p3 {background-color:hsl(120,100%,25%);}
#p4 {background-color:hsl(120,60%,70%);}
#p5 {background-color:hsl(290,100%,50%);}
#p6 {background-color:hsl(290,60%,70%);}
</style>
</head>
<body>

<h1>Define Colors With HSL Values</h1>

<p id="p1">Green</p>
<p id="p2">Light green</p>
<p id="p3">Dark green</p>
<p id="p4">Pastel green</p>
<p id="p5">Violet</p>
<p id="p6">Pastel violet</p>

</body>
</html>



HSLA Colors

HSLA color values are an extension of HSL color values with an alpha channel - which specifies the opacity 

for a color.

An HSLA color value is specified with: hsla(hue, saturation, lightness, alpha), where the alpha parameter 

defines the opacity. The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (fully opaque).

See the example below for different HSLA colors:

<!DOCTYPE html>
<html>
<head>
<style>
#p1 {background-color:hsla(120,100%,50%,0.3);}
#p2 {background-color:hsla(120,100%,75%,0.3);}
#p3 {background-color:hsla(120,100%,25%,0.3);}
#p4 {background-color:hsla(120,60%,70%,0.3);}
#p5 {background-color:hsla(290,100%,50%,0.3);}
#p6 {background-color:hsla(290,60%,70%,0.3);}
</style>
</head>
<body>

<h1>Define Colors With HSLA Values</h1>

<p id="p1">Green</p>
<p id="p2">Light green</p>
<p id="p3">Dark green</p>
<p id="p4">Pastel green</p>
<p id="p5">Violet</p>
<p id="p6">Pastel violet</p>

</body>
</html>




Opacity

The CSS opacity property sets the opacity for the whole element (both background color and text will be 

opaque/transparent).

The opacity property value must be a number between 0.0 (fully transparent) and 1.0 (fully opaque). 

The texts above will also be transparent. See example below for elements with specified opacity:


<!DOCTYPE html>
<html>
<head>
<style>
#p1 {background-color:rgb(255,0,0);opacity:0.6;}
#p2 {background-color:rgb(0,255,0);opacity:0.6;}
#p3 {background-color:rgb(0,0,255);opacity:0.6;}
#p4 {background-color:rgb(192,192,192);opacity:0.6;}
#p5 {background-color:rgb(255,255,0);opacity:0.6;}
#p6 {background-color:rgb(255,0,255);opacity:0.6;}
</style>
</head>
<body>

<h1>Define Colors With Opacity</h1>

<p id="p1">Red</p>
<p id="p2">Green</p>
<p id="p3">Blue</p>
<p id="p4">Grey</p>
<p id="p5">Yellow</p>
<p id="p6">Cerise</p>

</body>
</html>


<kbd>return</kbd>[Back to table of contents](#homepage)


-----------


## CSS Borders

CSS Border Style

The border-style property specifies what kind of border to display.

The following values are allowed:

dotted - Defines a dotted border
dashed - Defines a dashed border
solid - Defines a solid border
double - Defines a double border
groove - Defines a 3D grooved border. The effect depends on the border-color value
ridge - Defines a 3D ridged border. The effect depends on the border-color value
inset - Defines a 3D inset border. The effect depends on the border-color value
outset - Defines a 3D outset border. The effect depends on the border-color value
none - Defines no border
hidden - Defines a hidden border

The border-style property can have from one to four values (for the top border, right border, bottom border, 

and the left border).


<!DOCTYPE html>
<html>
<head>
<style>
p.dotted {border-style: dotted;}
p.dashed {border-style: dashed;}
p.solid {border-style: solid;}
p.double {border-style: double;}
p.groove {border-style: groove;}
p.ridge {border-style: ridge;}
p.inset {border-style: inset;}
p.outset {border-style: outset;}
p.none {border-style: none;}
p.hidden {border-style: hidden;}
p.mix {border-style: dotted dashed solid double;}
</style>
</head>
<body>

<h2>The border-style Property</h2>
<p>This property specifies what kind of border to display:</p>

<p class="dotted">A dotted border.</p>
<p class="dashed">A dashed border.</p>
<p class="solid">A solid border.</p>
<p class="double">A double border.</p>
<p class="groove">A groove border.</p>
<p class="ridge">A ridge border.</p>
<p class="inset">An inset border.</p>
<p class="outset">An outset border.</p>
<p class="none">No border.</p>
<p class="hidden">A hidden border.</p>
<p class="mix">A mixed border.</p>

</body>
</html>



Note: None of the OTHER CSS border properties (such as borders width, border colors, border sides, border 

shorthand, rounded borders) will have ANY effect unless the border-style property is set!


Border Width::

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-width: 5px;
}

p.two {
  border-style: solid;
  border-width: medium;
}

p.three {
  border-style: dotted;
  border-width: 2px;
}

p.four {
  border-style: dotted;
  border-width: thick;
}

p.five {
  border-style: double;
  border-width: 15px;
}

p.six {
  border-style: double;
  border-width: thick;
}
</style>
</head>
<body>

<h2>The border-width Property</h2>
<p>This property specifies the width of the four borders:</p>

<p class="one">Some text.</p>
<p class="two">Some text.</p>
<p class="three">Some text.</p>
<p class="four">Some text.</p>
<p class="five">Some text.</p>
<p class="six">Some text.</p>

<p><b>Note:</b> The "border-width" property does not work if it is used alone. 
Always specify the "border-style" property to set the borders first.</p>

</body>
</html>






CSS Border Width

The border-width property specifies the width of the four borders (top border, right border, bottom border, 

and left border) using px, pt, cm, em, etc. or using thin,medium, or thick. For specific side widths, two 

borders are specified. The first represents top and bottom border with, while the second represents the 

width for the sides borders. 



<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-width: 5px 20px; /* 5px top and bottom, 20px on the sides */
}

p.two {
  border-style: solid;
  border-width: 20px 5px; /* 20px top and bottom, 5px on the sides */
}

p.three {
  border-style: solid;
  border-width: 25px 10px 4px 35px; /* 25px top, 10px right, 4px bottom and 35px left */
}
</style>
</head>
<body>

<h2>The border-width Property</h2>
<p>The border-width property can have from one to four values (for the top border, right border, bottom 

border, and the left border):</p>

<p class="one">Some text.</p>
<p class="two">Some text.</p>
<p class="three">Some text.</p>

</body>
</html>

CSS Border Color::

The border-color property is used to set the color of the four borders using name ( e.g. red), HEX value 

(e.g. #ff0000), RGB value (e.g. rgb(255,0,0), and HSL value (e.g. hsl (0, 100%, 50%), and transparency

(specified using alpha value). 


Note: The elements's color is the default border-color whenever you did not set the border color.

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: red;
}

p.two {
  border-style: solid;
  border-color: green;
} 

p.three {
  border-style: dotted;
  border-color: blue;
} 
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>This property specifies the color of the four borders:</p>

<p class="one">A solid red border</p>
<p class="two">A solid green border</p>
<p class="three">A dotted blue border</p>

<p><b>Note:</b> The "border-color" property does not work if it is used alone. Use the "border-style" 

property to set the borders first.</p>

</body>
</html>



Specific Side Colors


The border-color property can have from one to four values (for the top border, right border, bottom border, 

and the left border). 


<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: red green blue yellow; /* red top, green right, blue bottom and yellow left */
}
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>The border-color property can have from one to four values (for the top border, right border, bottom 

border, and the left border):</p>

<p class="one">A solid multicolor border</p>

</body>
</html>


Hexadecimal (HEX) Values

The color of the border can also be specified using HEX values. 


<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: #ff0000; /* red */
}

p.two {
  border-style: solid;
  border-color: #0000ff; /* blue */
}

p.three {
  border-style: solid;
  border-color: #bbbbbb; /* grey */
}
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>The color of the border can also be specified using a hexadecimal value (HEX):</p>

<p class="one">A solid red border</p>
<p class="two">A solid blue border</p>
<p class="three">A solid grey border</p>

</body>
</html>



RGB Values

RGB values can also be used to specify color. 

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: rgb(255, 0, 0); /* red */
}

p.two {
  border-style: solid;
  border-color: rgb(0, 0, 255); /* blue */
}

p.three {
  border-style: solid;
  border-color: rgb(187, 187, 187); /* grey */
}
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>The color of the border can also be specified using RGB values:</p>

<p class="one">A solid red border</p>
<p class="two">A solid blue border</p>
<p class="three">A solid grey border</p>

</body>
</html>


HSL Values

HSL values can be used to specify.

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: hsl(0, 100%, 50%); /* red */
}

p.two {
  border-style: solid;
  border-color: hsl(240, 100%, 50%); /* blue */
}

p.three {
  border-style: solid;
  border-color: hsl(0, 0%, 73%); /* grey */
}
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>The color of the border can also be specified using HSL values:</p>

<p class="one">A solid red border</p>
<p class="two">A solid blue border</p>
<p class="three">A solid grey border</p>

</body>
</html>



CSS Border Sides::

CSS Border - Individual Sides

You can use some CSS properties to specify the type of border each side (top, right, bottom, and left) has


<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-top-style: dotted;
  border-right-style: solid;
  border-bottom-style: dotted;
  border-left-style: solid;
}
</style>
</head>
<body>

<h2>Individual Border Sides</h2>
<p>2 different border styles.</p>

</body>
</html>


The code above can also be written as (dotted and solid represent top+bottom, and left+right respectively: 

<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-style: dotted solid;
}
</style>
</head>
<body>

<h2>Individual Border Sides</h2>
<p>2 different border styles.</p>

</body>
</html>


Border style explanation : 
If the border-style property has four values:

    border-style: dotted solid double dashed;
        top border is dotted
        right border is solid
        bottom border is double
        left border is dashed

If the border-style property has three values:

    border-style: dotted solid double;
        top border is dotted
        right and left borders are solid
        bottom border is double

If the border-style property has two values:

    border-style: dotted solid;
        top and bottom borders are dotted
        right and left borders are solid

If the border-style property has one value:

    border-style: dotted;
        all four borders are dotted


The above also works with border-width and border-color

See code below for example of practical use of the border styling parameters

<!DOCTYPE html>
<html>
<head>
<style>
body {
  text-align: center;
}
/* Four values */
p.four {
  border-style: dotted solid double dashed;
}

/* Three values */
p.three {
  border-style: dotted solid double;
}

/* Two values */
p.two {
  border-style: dotted solid;
}

/* One value */
p.one {
  border-style: dotted;
}
</style>
</head>
<body>

<h2>Individual Border Sides</h2>
<p class="four">4 different border styles.</p>
<p class="three">3 different border styles.</p>
<p class="two">2 different border styles.</p>
<p class="one">1 border style.</p>

</body>
</html>

CSS Border-Shorthand property::
Enable shortening of the border styling codes. The 'border' property is a shorthand for individual border 

properties, as shown below (for example)


    border-width
    border-style (required)
    border-color
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border: 5px solid red;
}
</style>
</head>
<body>

<h2>The border Property</h2>

<p>This property is a shorthand property for border-width, border-style, and border-color.</p>

</body>
</html>



Border properties can also be specified for each side:
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-left: 6px solid red;
  background-color: lightgrey;
}
</style>
</head>
<body>

<h2>The border-left Property</h2>
<p>This property is a shorthand property for border-left-width, border-left-style, and border-left-

color.</p>

</body>
</html>


To repeat the same for bottom border:

<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-bottom: 6px solid red;
  background-color: lightgrey;
}
</style>
</head>
<body>

<h2>The border-bottom Property</h2>
<p>This property is a shorthand property for border-bottom-width, border-bottom-style, and border-bottom-

color.</p>

</body>
</html>


CSS Rounded Borders::
Use border radius to add rounded borders to an element


<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  border: 2px solid red;
}

p.round1 {
  border: 2px solid red;
  border-radius: 5px;
}

p.round2 {
  border: 2px solid red;
  border-radius: 8px;
}

p.round3 {
  border: 2px solid red;
  border-radius: 12px;
}
</style>
</head>
<body>

<h2>The border-radius Property</h2>
<p>This property is used to add rounded borders to an element:</p>

<p class="normal">Normal border</p>
<p class="round1">Round border</p>
<p class="round2">Rounder border</p>
<p class="round3">Roundest border</p>

</body>
</html>


NB: Some shortcuts on border styling

To set all properties of top border in one go:
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-style: solid;
  border-top: thick double #ff0000;
}
</style>
</head>
<body>

<p>This is some text in a paragraph.</p>

</body>
</html>


To set the style of the bottom border

<!DOCTYPE html>
<html>
<head>
<style>
p {border-style: solid;}
p.none {border-bottom-style: none;}
p.dotted {border-bottom-style: dotted;}
p.dashed {border-bottom-style: dashed;}
p.solid {border-bottom-style: solid;}
p.double {border-bottom-style: double;}
p.groove {border-bottom-style: groove;}
p.ridge {border-bottom-style: ridge;}
p.inset {border-bottom-style: inset;}
p.outset {border-bottom-style: outset;}
</style>
</head>
<body>

<p class="none">No bottom border.</p>
<p class="dotted">A dotted bottom border.</p>
<p class="dashed">A dashed bottom border.</p>
<p class="solid">A solid bottom border.</p>
<p class="double">A double bottom border.</p>
<p class="groove">A groove bottom border.</p>
<p class="ridge">A ridge bottom border.</p>
<p class="inset">An inset bottom border.</p>
<p class="outset">An outset bottom border.</p>

</body>
</html>



To set the width of the left border

<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-style: solid;
  border-left-width: 15px;
}
</style>
</head>
<body>

<p><b>Note:</b> The "border-left-width" property does not work if it is used alone. Use the "border-style" 

property to set the borders first.</p>

</body>
</html>


To set the color of the four borders:

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  
  border-color: #0000ff;
}

p.two {
  border-style: solid;
  border-color: #ff0000 #0000ff;
}

p.three {
  border-style: solid;
  border-color: #ff0000 #00ff00 #0000ff;
}

p.four {
  border-style: solid;
  border-color: #ff0000 #00ff00 #0000ff rgb(250,0,255);
}
</style>
</head>
<body>

<p class="one">One-colored border!</p>
<p class="two">Two-colored border!</p>
<p class="three">Three-colored border!</p>
<p class="four">Four-colored border!</p>
<p><b>Note:</b> The "border-color" property does not work if it is used alone. Use the "border-style" 

property to set the borders first.</p>

</body>
</html>


To set the color of the right border:
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-style: solid;
  border-right-color: #ff0000;
}
</style>
</head>
<body>

<p>This is some text in a paragraph.</p>

</body>
</html>


All CSS Border Properties
Property 	Description
border 	Sets all the border properties in one declaration
border-bottom 	Sets all the bottom border properties in one declaration
border-bottom-color 	Sets the color of the bottom border
border-bottom-style 	Sets the style of the bottom border
border-bottom-width 	Sets the width of the bottom border
border-color 	Sets the color of the four borders
border-left 	Sets all the left border properties in one declaration
border-left-color 	Sets the color of the left border
border-left-style 	Sets the style of the left border
border-left-width 	Sets the width of the left border
border-radius 	Sets all the four border-*-radius properties for rounded corners
border-right 	Sets all the right border properties in one declaration
border-right-color 	Sets the color of the right border
border-right-style 	Sets the style of the right border
border-right-width 	Sets the width of the right border
border-style 	Sets the style of the four borders
border-top 	Sets all the top border properties in one declaration
border-top-color 	Sets the color of the top border
border-top-style 	Sets the style of the top border
border-top-width 	Sets the width of the top border
border-width 	Sets the width of the four borders

<kbd>return</kbd>[Back to table of contents](#homepage)

-----
## CSS Margins

To create space around an element outside of specified borders. the 'margin' gives control over the margin 

around an element. You can also set margin on the four sides. There are properties for setting the margin 

for each side of an element (top, right, bottom, and left).

The code below add a 70px margin space around <p> element. 

<!DOCTYPE html>
<html>
<head>
<style>
div {
  margin: 70px;
  border: 1px solid #4CAF50;
}
</style>
</head>
<body>

<h2>CSS Margins</h2>
<div>This element has a margin of 70px.</div>

</body>
</html>



Margin - Individual Sides::

CSS has properties for specifying the margin for each side of an element:

    margin-top
    margin-right
    margin-bottom
    margin-left

All the margin properties can have the following values:

    auto - the browser calculates the margin
    length - specifies a margin in px, pt, cm, etc.
    % - specifies a margin in % of the width of the containing element
    inherit - specifies that the margin should be inherited from the parent element

Tip: Negative values are allowed.

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>Using individual margin properties</h2>

<div>This div element has a top margin of 100px, a right margin of 150px, a bottom margin of 100px, and a 

left margin of 80px.</div>

</body>
</html>



Margin Shorthand Property

To shorten the code, it is possible to specify all the margin properties in one property.

The margin property is a shorthand property for the following individual margin properties:

    margin-top
    margin-right
    margin-bottom
    margin-left

So, here is how it works:

If the margin property has four values:

    margin: 25px 50px 75px 100px;
        top margin is 25px
        right margin is 50px
        bottom margin is 75px
        left margin is 100px


Example:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin: 25px 50px 75px 100px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The margin shorthand property - 4 values</h2>

<div>This div element has a top margin of 25px, a right margin of 50px, a bottom margin of 75px, and a left 

margin of 100px.</div>

<hr>

</body>
</html>


If the margin property has three values:

    margin: 25px 50px 75px;
        top margin is 25px
        right and left margins are 50px
        bottom margin is 75px

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin: 25px 50px 75px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The margin shorthand property - 3 values</h2>

<div>This div element has a top margin of 25px, a right and left margin of 50px, and a bottom margin of 

75px.</div>

<hr>

</body>
</html>


If the margin property has two values:

    margin: 25px 50px;
        top and bottom margins are 25px
        right and left margins are 50px


<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin: 25px 50px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The margin shorthand property - 2 values</h2>

<div>This div element has a top and bottom margin of 25px, and a right and left margin of 50px.</div>

<hr>

</body>
</html>



If the margin property has one value:

    margin: 25px;
        all four margins are 25px




<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin: 25px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The margin shorthand property - 1 value</h2>

<div>This div element has a top, bottom, left, and right margin of 25px.</div>

<hr>

</body>
</html>




The margin: auto,  Value

You can set the margin property to auto to horizontally center the element within its container.

The element will then take up the specified width, and the remaining space will be split equally between the 

left and right margins.


<!DOCTYPE html>
<html>
<head>
<style>
div {
  width:300px;
  margin: auto;
  border: 1px solid red;
}
</style>
</head>
<body>

<h2>Use of margin:auto</h2>
<p>You can set the margin property to auto to horizontally center the element within its container. The 

element will then take up the specified width, and the remaining space will be split equally between the 

left and right margins:</p>

<div>
This div will be horizontally centered because it has margin: auto;
</div>

</body>
</html>


The inherit Value for margin
To let the left margin of the <p class="ex1"> element be inherited from the parent element.


<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid red;
  margin-left: 100px;
}

p.ex1 {
  margin-left: inherit;
}
</style>
</head>
<body>

<h2>Use of the inherit value</h2>
<p>Let the left margin be inherited from the parent element:</p>

<div>
<p class="ex1">This paragraph has an inherited left margin (from the div element).</p>
</div>

</body>
</html>


CSS Margin Collapse::
Enables you to collapse 2 margins into one.

Margin Collapse

Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest 

of the two margins.

This does not happen on left and right margins! Only top and bottom margins!


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  margin: 0 0 50px 0;
}

h2 {
  margin: 20px 0 0 0;
}
</style>
</head>
<body>

<p>In this example the h1 element has a bottom margin of 50px and the h2 element has a top margin of 20px. 

So, the vertical margin between h1 and h2 should have been 70px (50px + 20px). However, due to margin 

collapse, the actual margin ends up being 50px.</p>

<h1>Heading 1</h1>
<h2>Heading 2</h2>

</body>
</html>


In the example above, the <h1> element has a bottom margin of 50px and the <h2> element has a top margin set 

to 20px.

Common sense would seem to suggest that the vertical margin between the <h1> and the <h2> would be a total 

of 70px (50px + 20px). But due to margin collapse, the actual margin ends up being 50px.



All CSS Margin Properties
Property 	Description
margin 	A shorthand property for setting the margin properties in one declaration
margin-bottom 	Sets the bottom margin of an element
margin-left 	Sets the left margin of an element
margin-right 	Sets the right margin of an element
margin-top 	Sets the top margin of an element

<kbd>return</kbd>[Back to table of contents](#homepage)

-----



## CSS Padding

CSS 'padding' is used to create spaces outside an element inside any specified borders. To use css padding, 

see below for an example. You can also use CSS to set padding for all the four sides of a CSS element. 

<!DOCTYPE html>
<html>
<head>
<style>
div {
  padding: 100px;
  border: 1px solid #4CAF50;
}
</style>
</head>
<body>

<h2>CSS Padding</h2>
<div>This element has a padding of 70px.</div>

</body>
</html>



Padding - Individual Sides


CSS has properties for specifying the padding for each side of an element:

    padding-top
    padding-right
    padding-bottom
    padding-left

All the padding properties can have the following values:

    length - specifies a padding in px, pt, cm, etc.
    % - specifies a padding in % of the width of the containing element
    inherit - specifies that the padding should be inherited from the parent element

Note: Negative values are not allowed.


For the used of padding on all the four sides, see below for example of use case:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  background-color: lightblue;
  padding-top: 50px;
  padding-right: 30px;
  padding-bottom: 50px;
  padding-left: 80px;
}
</style>
</head>
<body>

<h2>Using individual padding properties</h2>

<div>This div element has a top padding of 50px, a right padding of 30px, a bottom padding of 50px, and a 

left padding of 80px.</div>

</body>
</html>




Padding - Shorthand Property

These properties enable shortening padding properties in one property. For example: 


The padding property is a shorthand property for the following individual padding properties:

    padding-top
    padding-right
    padding-bottom
    padding-left

So, here is how it works:

If the padding property has four values:

    padding: 25px 50px 75px 100px;
        top padding is 25px
        right padding is 50px
        bottom padding is 75px
        left padding is 100px


For example:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 25px 50px 75px 100px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The padding shorthand property - 4 values</h2>

<div>This div element has a top padding of 25px, a right padding of 50px, a bottom padding of 75px, and a 

left padding of 100px.</div>

</body>
</html>


For padding properties having three values:

If the padding property has three values:

    padding: 25px 50px 75px;
        top padding is 25px
        right and left paddings are 50px
        bottom padding is 75px


For example,


<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 25px 50px 75px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The padding shorthand property - 3 values</h2>

<div>This div element has a top padding of 25px, a right and left padding of 50px, and a bottom padding of 

75px.</div>

</body>
</html>




For padding properties with two values,

If the padding property has two values:

    padding: 25px 50px;
        top and bottom paddings are 25px
        right and left paddings are 50px


For example:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 25px 50px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The padding shorthand property - 2 values</h2>

<div>This div element has a top and bottom padding of 25px, and a right and left padding of 50px.</div>

</body>
</html>



When padding property has one value:

If the padding property has one value:

    padding: 25px;
        all four paddings are 25px


For example,
<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 25px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The padding shorthand property - 1 value</h2>

<div>This div element has a top, bottom, left, and right padding of 25px.</div>

</body>
</html>




Padding and Element Width

The width element specify width of element's content area ( the area inside the padding, border, and margin 

of the element accordingt to the box model). For an element witrh specified width, the padding of such 

element is added to the value of the specified width ( an often undesirable result).


For example,

<!DOCTYPE html>
<html>
<head>
<style>
div.ex1 {
  width: 300px;
  background-color: yellow;
}

div.ex2 {
  width: 300px;
  padding: 25px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>Padding and element width</h2>

<div class="ex1">This div is 300px wide.</div>
<br>

<div class="ex2">The width of this div is 350px, even though it is defined as 300px in the CSS.</div>

</body>
</html>


Whenever you need to maintain the widht, the box-sizing property is used to keep width constant irrespective 

of the amount of padding. This effect will collapse available space for the element inwards of the defined 

borders. 

 
For example.

<!DOCTYPE html>
<html>
<head>
<style>
div.ex1 {
  width: 300px;
  background-color: yellow;
}

div.ex2 {
  width: 300px;
  padding: 25px;
  box-sizing: border-box;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>Padding and element width - with box-sizing</h2>

<div class="ex1">This div is 300px wide.</div>
<br>

<div class="ex2">The width of this div remains at 300px, in spite of the 50px of total left and right 

padding, because of the box-sizing: border-box property.
</div>

</body>
</html>



Other padding examples,


To set the left padding of an element,


<!DOCTYPE html>
<html>
<head>
<style>
p.padding {
  padding-left: 2cm;
}
p.padding2 {
  padding-left: 50%;
}
</style>
</head>
<body>

<h1>The padding-left Property</h1>

<p>This is a text with no left padding.</p>
<p class="padding">This text has a left padding of 2 cm.</p>
<p class="padding2">This text has a left padding of 50%.</p>

</body>
</html>



To set the right padding,

<!DOCTYPE html>
<html>
<head>
<style>
p.padding {
  padding-right: 2cm;
}

p.padding2 {
  padding-right: 50%;
}
</style>
</head>
<body>

<h1>The padding-right Property</h1>

<p>This is a text with no right padding. This is a text with no right padding. This is a text with no right 

padding.</p>
<p class="padding">This text has a right padding of 2 cm. This text has a right padding of 2 cm. This text 

has a right padding of 2 cm.</p>
<p class="padding2">This text has a right padding of 50%. This text has a right padding of 50%. This text 

has a right padding of 50%.</p>

</body>
</html>


To set the top padding,

<!DOCTYPE html>
<html>
<head>
<style>
p.padding {
  padding-top: 2cm;
}

p.padding2 {
  padding-top: 50%;
}
</style>
</head>
<body>

<h1>The padding-top Property</h1>

<p>This is a text with no top padding. This is a text with no top padding. This is a text with no top 

padding.</p>
<p class="padding">This text has a top padding of 2 cm. This text has a top padding of 2 cm. This text has a 

top padding of 2 cm.</p>
<p class="padding2">This text has a top padding of 50%. This text has a top padding of 50%. This text has a 

top padding of 50%.</p>

</body>
</html>


To set the bottom padding,


<!DOCTYPE html>
<html>
<head>
<style>
p.padding {
  padding-bottom:2cm;
}

p.padding2 {
  padding-bottom:50%;
}
</style>
</head>
<body>

<h1>The padding-bottom Property</h1>

<p>This is a text with no bottom padding. This is a text with no bottom padding. This is a text with no 

bottom padding.</p>
<p class="padding">This text has a bottom padding of 2 cm. This text has a bottom padding of 2 cm. This text 

has a bottom padding of 2 cm.</p>
<p class="padding2">This text has a bottom padding of 50%. This text has a bottom padding of 50%. This text 

has a bottom padding of 50%.</p>

</body>
</html>



All CSS Padding Properties summary
Property 	Description
padding 	A shorthand property for setting all the padding properties in one declaration
padding-bottom 	Sets the bottom padding of an element
padding-left 	Sets the left padding of an element
padding-right 	Sets the right padding of an element
padding-top 	Sets the top padding of an element

<kbd>return</kbd>[Back to table of contents](#homepage)

