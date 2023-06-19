## HTML IMAGES

## IMAGES

```<img src="pic_trulli.jpg" alt="Italian Trulli">```

Image tag is used to insert images in a webpage. Images are linked to a webpage not embeded. 

SRC attributes
src - Specifies the path to the image
alt - Specifies an alternate text for the image

Syntax
```<img src="url" alt="alternatetext">``` 

Browsers get image from a web server and inserts into the page each time yu load. Image stays in same spot in relation to a webpage...else the alt text shows up to indicate that the link is brocken.

**Value of alt attribute shows in cases where: because of slow connection, an error in the src attribute, or if the user uses a screen reader which reads html code and reads out for the user...usually used by the visually impaired people.

**You can also specify width and height in the style attribute of the image

 ```<img src="img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">``` 

**With and height attribute as width and height attribute...which is always in pixels
 ```<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">``` 

**It is better to use style attribute so the stylesheet does not end up changing image size.

```
<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 100%;
}
</style>
</head>
<body>

<img src="html5.gif" alt="HTML5 Icon" width="128" height="128">

<img src="html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">

</body>
</html> 
```

**For images in the subfolder, you must include the folder name

```<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">``` 

If your  site point to an external image on another server, specify full URL to point to the image.

 ```mg src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">``` 

NB on external images: Might be removed by site owner anytime. Also getting permission may be necessary to avoid copyright violation

**Animated Images:: HTML allows GIFs

```<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">``` 

**Image as a tag:: Put <img> tag inside the <a> tag

```
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a> 
```
**Let image float to the right or to the left of a text using CSS float property
```
<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
The image will float to the right of the text.</p>

<p><img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
The image will float to the left of the text.</p> 
```
**Common image formats supported on a website

bbreviation 	File Format 	File Extension
APNG 	Animated Portable Network Graphics 	.apng
GIF 	Graphics Interchange Format 	.gif
ICO 	Microsoft Icon 	.ico, .cur
JPEG 	Joint Photographic Expert Group image 	.jpg, .jpeg, .jfif, .pjpeg, .pjp
PNG 	Portable Network Graphics 	.png
SVG 	Scalable Vector Graphics 	.svg


**Loading large images takes time and can slow down your webpage...so use images carefully.

<kbd>return</kbd>[Back to table of contents](#homepage)


------- 



## HTML IMAGES

## IMAGES

```<img src="pic_trulli.jpg" alt="Italian Trulli">```

Image tag is used to insert images in a webpage. Images are linked to a webpage not embeded. 

SRC attributes
src - Specifies the path to the image
alt - Specifies an alternate text for the image

Syntax
```<img src="url" alt="alternatetext">``` 

Browsers get image from a web server and inserts into the page each time yu load. Image stays in same spot in relation to a webpage...else the alt text shows up to indicate that the link is brocken.

**Value of alt attribute shows in cases where: because of slow connection, an error in the src attribute, or if the user uses a screen reader which reads html code and reads out for the user...usually used by the visually impaired people.

**You can also specify width and height in the style attribute of the image

 ```<img src="img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">``` 

**With and height attribute as width and height attribute...which is always in pixels
 ```<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">``` 

**It is better to use style attribute so the stylesheet does not end up changing image size.

```
<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 100%;
}
</style>
</head>
<body>

<img src="html5.gif" alt="HTML5 Icon" width="128" height="128">

<img src="html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">

</body>
</html> 
```

**For images in the subfolder, you must include the folder name

```<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">``` 

If your  site point to an external image on another server, specify full URL to point to the image.

 ```mg src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">``` 

NB on external images: Might be removed by site owner anytime. Also getting permission may be necessary to avoid copyright violation

**Animated Images:: HTML allows GIFs

```<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">``` 

**Image as a tag:: Put <img> tag inside the <a> tag

```
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a> 
```
**Let image float to the right or to the left of a text using CSS float property
```
<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
The image will float to the right of the text.</p>

<p><img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
The image will float to the left of the text.</p> 
```
**Common image formats supported on a website

bbreviation 	File Format 	File Extension
APNG 	Animated Portable Network Graphics 	.apng
GIF 	Graphics Interchange Format 	.gif
ICO 	Microsoft Icon 	.ico, .cur
JPEG 	Joint Photographic Expert Group image 	.jpg, .jpeg, .jfif, .pjpeg, .pjp
PNG 	Portable Network Graphics 	.png
SVG 	Scalable Vector Graphics 	.svg


**Loading large images takes time and can slow down your webpage...so use images carefully.

<kbd>return</kbd>[Back to table of contents](#homepage)

## IMAGE MAP
Image Maps::Allows you to perform actions depending on where in image  you click. You need an image, some html code that describes the clickable area. 

The image: Inserted using image tag, but you must add usemap attribute in this case.

```
<img src="workplace.jpg" alt="Workplace" usemap="#workmap">
```

-The usemap value starts with a hash tag # followed by the name of the image map, and is used to create a relationship between the image and the image map.

You can use any image as an image map.

-add a ```<map>``` element linked to the image using the name attribute.

```
<map name="workmap">
```
name attribute must have the same value as the <img>'s usemap attribute

-Add clickable area to the image: You define the clickable area using an <area> element.
* Define shape of the clickable area using any of these values: 
 rect - defines a rectangular region
 circle - defines a circular region
 poly - defines a polygonal region
 default - defines the entire region

-Define coordinate to be able to place the clickable area onto the image.

```
Shape="rect"
```
The coordinates for ```shape="rect"``` come in pairs, one for the x-axis (distance from left) and one for the y-axis(distance from top).

So, the coordinates 34,44 is located 34 pixels from the left margin and 44 pixels from the top:

The coordinates 270,350 is located 270 pixels from the left margin and 350 pixels from the top:


```Shape="circle"```

To add a circle area, first locate the coordinates of the center of the circle:

337,300  

then specify the radius: 44 pixels

** 
```
<area shape="circle" coords="337, 300, 44" href="coffee.htm"> 
``` 
```Shape=poly"```

The ```shape="poly"``` contains several coordinate points, which creates a shape formed with straight lines (a polygon).

This can be used to create any shape. Such as a croissant. You have to find x and y coordinates for all edges of the croissant.

* Each point has x and y...specify all the coordinates around the perimeter of the polygonal shape. 

 ```
 <area shape="poly" coords="140,121,181,116,204,160,204,222,191,270,140,329,85,355,58,352,37,322,40,259,103,161,128,147" href="croissant.htm">
 ``` 
**You can also trigger a JS function by clicking the poissant shape.
Add a click event to the <area> element to execute a JavaScript function:

```
 <map name="workmap">
  <area shape="circle" coords="337,300,44" onclick="myFunction()">
</map>

<script>
function myFunction() {
  alert("You clicked the coffee cup!");
}
</script> 
```
You can use href with the function to inform user to confirm what they are trying to do before they follow the hyperlink on the picture.

**Image Map summary: =

```
<img> 	Defines an image
<map> 	Defines an image map
<area> 	Defines a clickable area inside an image map
<picture> 	Defines a container for multiple image resources
```
<kbd>return</kbd>[Back to table of contents](#homepage)

## Background Images

Background Images: Repeats itself if it is smaller 

*Add background image on an HTML element using style attribute and css background-image.
```
 <div style="background-image: url('img_girl.jpg');"> 
```

**You can also specify background image in the style element of the head section
```
 <style>
div {
  background-image: url('img_girl.jpg');
}
</style> 
```

**Adding background image for an entire page:specify background image on the body element
```
<style>
body {
  background-image: url('img_girl.jpg');
}
</style> 
```

**Background image repeat:: Background image smaller than the element will repeat itself, horizontally and vertically,until it reaches the end of the element. 

```
<style>
body {
  background-image: url('img_girl.jpg');
}
</style> 

**You can set background repeat property to no repeat to prevent the background image from repeating itself. 

 <style>
body {
  background-image: url('example_img_girl.jpg');
  background-repeat: no-repeat;
}
</style> 
```

* Background Cover: You can set background-size property to cover to make background image to cover the entire element. set the background-attachment property to fixed to make sure the entire element is always covered...This keeps image original proportions. 

```
<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
```
** Background stretch::  Allows you to make the background image to stretch to fit the entire element. Set background-size property to 100% 100%

```
 <style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 100% 100%;
}
</style> 
```

<kbd>return</kbd>[Back to table of contents](#homepage)


------



## CSS HOW TO ADD CSS

Browser formats html using the information in the style sheet or <style>


External CSS::

It is a file that you can use to change the style of an entire website. Each page of the website then 

include <link> , in the <head> section, which contains a link to the external styling sheet that controls 

the style of the whole document. You can create the external file with any text editor. This file should be 

saved with a .css extension and the file must not contain any HTML tags. 


when "mystyle.css" contains the code:

```
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
  
```


The mystyle can be inherited below:
  
```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

NB: No space between property value and it's unit. I.e use: 20px not 20 px


Internal CSS::

Can be used if one single HTML page has a unique style. You should define inside the ```<style>``` element, inside 

the ```<head>``` section. Example of internal CSS is shown below:

```
!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
} 
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```


Inline CSS::

You can use an inline style to apply unique style to just a single element. To use inline styles, add the 

style attribute to the appropriate element. Style attribute can contain any of the CSS properties.

```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```

NB: And inline style denies you the benefits of a style sheet since you now have to edit the styling of 

elements individually. Only use CSS inline when necessary



Multiple Style Sheets::

If you have styles for same element in different style sheet, the last read style of sheet for the elements 

is applied to the element.


if mystyle.css contains:

```
h1 {
  color: navy;
}

and internal style sheet contains the following:


h1 {
  color: orange;   
}
```

Case A: Internal style defined after the link to external style sheet,```<h1>``` elements will take an orange 

color since the internal style comes last

```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<style>
h1 {
  color: orange;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>The style of this document is a combination of an external stylesheet, and internal style</p>

</body>
</html>
```

Case B: If the internal style is defined before the link the external style sheet, then the ```<h1>``` elements 

will take the navy color defined in the style sheet. 

```
<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  color: orange;
}
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>The style of this document is a combination of an external stylesheet, and internal style</p>

</body>
</html>
```


Cascading Order::

When an HTML element has more than one style specified for it, all styles will 'cascade' into a new virtual 

style sheet according to the rules below 1. has highest priority and 3. has the least.


1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default

Inline style is highest priority and can override external styles and browser defaults.

<kbd>return</kbd>[Back to table of contents](#homepage)
  
-------

## CSS COMMENTS

  

They do not show in the browser but improve code readability:


They may help you edit the source code later on. The comment is placed inside <style> element, starts with 

```/* and ends with */```   and you can have the comment anywhere in the code you like.

```
 /* This is a single-line comment */
p {
  color: red;
} 


/* This is
a multi-line
comment */


p {
  color: red;
} 
```

HTML and CSS Comments

The HTML comment is: ```<!--this is a comment--!>```. You can combine HTML style with a CSS for an element:

```
<!DOCTYPE html>
<html>
<head>
<style>
p {
  color: red; /* Set text color to red */
}
</style>
</head>
<body>

<h2>My Heading</h2>

<!-- These paragraphs will be red -->
<p>Hello World!</p>
<p>This paragraph is styled with CSS.</p>
<p>HTML and CSS comments are not shown in the output.</p>

</body>
</html>
```
<kbd>return</kbd>[Back to table of contents](#homepage)


--------


## CSS COLORS


Colors:: 

You can specify color with predefined color names: RGB, HEX, HSL, RGBA, HSLA.


CSS Color names: There are 140 supported standard color names. See the link below for the full list.



CSS Background Color: Set the background color as shown below
  
```
<h1 style="background-color:DodgerBlue;">Hello World</h1>

<p style="background-color:Tomato;">
```

CSS Text Color: You can also set the color of the text as shown below:

```
<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Ut wisi enim...</p> 
```

CSS Border Color: Use can use this to change the color of the border (the box around a text). The

```
<body>

<h1 style="border: 2px solid Tomato;">Hello World</h1>

<h1 style="border: 2px solid DodgerBlue;">Hello World</h1>

<h1 style="border: 2px solid Violet;">Hello World</h1>

</body>
```

CSS Color values

You can specify color using RGB values, HEX values, HSL values, and RGBA values, and HSLA values.



The three below are still tomato colors

```
rgb(255, 99, 71)
#ff6347
hsl(9, 100%, 64%)
```



The below are tomato with 50% transparency:

```
rgba(255, 99, 71, 0.5)
hsla(9, 100%, 64%, 0.5)
```

See the application below:
```
<!DOCTYPE html>
<html>
<body>

<p>Same as color name "Tomato":</p>

<h1 style="background-color:rgb(255, 99, 71);">rgb(255, 99, 71)</h1>
<h1 style="background-color:#ff6347;">#ff6347</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">hsl(9, 100%, 64%)</h1>

<p>Same as color name "Tomato", but 50% transparent:</p>
<h1 style="background-color:rgba(255, 99, 71, 0.5);">rgba(255, 99, 71, 0.5)</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">hsla(9, 100%, 64%, 0.5)</h1>

<p>In addition to the predefined color names, colors can be specified using RGB, HEX, HSL, or even 

transparent colors using RGBA or HSLA color values.</p>

</body>
</html>
```



CSS RGB::

RGB Value: RGB rep red, green, and blue light sources

```
format: rgb(red_value,green_value,blue_value)

```
Each of the color values range from 0 to 255

```red= rgb(255,0,0);``` since red color is max while blue and green are absent.


```black=rgb(0,0,0);``` since there is absence of light

```white=rgb(255,255,255);``` since there is an excess of all the lights...no color shows

```grey=rgb(x,x,x);``` equal color values produce grey. So, you have black at ```rgb(0,0,0)```, and white at ```rgb(255,255,255)```.Every other equal mix between 0 and 255 is grey but to different extent. The closer the equal 

values are to zero the darker the grey color is. 

  
RGBA Value: It includes alpha channel ( a measure of opacity) for each of the colors. 

format: rgba(red_value,green_value,blue_value,alpha)

Fully transparent: alpha=0.0
Not transparent at all: alpha=1.0



CSS HEX COLORS::

hexadecimal color format: #RRGGBB   (RR=RED, GG=GREEN, BB=BLUE)

The hexadecimal integers specify the component of the color. 


HEX Value ranges from  00 to ff, just like decimal ranges from 0 to 255


#ff0000=red because red is set to max while green and blue are set to zero. 

#000000: black because no color light present

#ffffff: white because max color light present in all the cases.

Any equal values between 000000 and ffffff gives grey

#787878=grey


3 Digit HEX Value: It is a short form ofsome 6 digit hex codes 
The format of the 3 digit hex code is: #rgb

You can only use the 3digit hex code when both red, green, and blue component values are the same for 

example:

body {
  background-color: #fc9; /* same as #ffcc99 */
}

h1 {
  color: #f0f; /* same as #ff00ff */
}

p {
  color: #b58; /* same as #bb5588 */
}




CSS HSL Colors::

HSL = Hue, Saturation, Lightness


format: hsl(hue, saturation, lightness)


Hue=Degree on color wheel from  0 to 360 ( Hue=0 (Red), Hue=120(Green), Hue=240(Blue))

Saturation: Percentage value from shade of gray (0%) to full color(100%)

LIghtness: Percentage value from Black(0%) to white(100%), to neither white or black (50%)



Saturation::: Intensity of a color. Pure color+no shades of gray=100%, Gray+invisible color=50%, Completely 

gray=0% and you can no longer see the color


Lightness: CAn be described by how much light you want give the color. No light( black)=0%, Neither light 

nor dark=50%, full lightness (white) = 100%


Shades of gray involves setting hue and saturation to zero and then adjusting lightness from 0% to 100% to 

get darker/lighter shades. 

hsl(0%,0%,0%)=black

hsl(0%,0%,100%)=white
hsl(0%,0%,47%)=grey


HsLA Value::: They are an extension of the HSL color values by including an alpha channel

hsla(hue, saturation, lightness, alpha)


<kbd>return</kbd>[Back to table of contents](#homepage)


---------


## CSS Box Model

All html elements can be considered to be boxes. The box model wraps around every HTML element and consists 

of margins, borders, padding, and the actual content ( when you go from outside the element to inside the 

element. 



Explanation of the different parts:

    Content - The content of the box, where text and images appear
    Padding - Clears an area around the content. The padding is transparent
    Border - A border that goes around the padding and content
    Margin - Clears an area outside the border. The margin is transparent

For example,

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: lightgrey;
  width: 300px;
  border: 15px solid green;
  padding: 50px;
  margin: 20px;
}
</style>
</head>
<body>

<h2>Demonstrating the Box Model</h2>

<p>The CSS box model is essentially a box that wraps around every HTML element. It consists of: borders, 

padding, margins, and the actual content.</p>

<div>This text is the content of the box. We have added a 50px padding, 20px margin and a 15px green border. 

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 

Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 

Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est 

laborum.</div>

</body>
</html>


Width and height of an element

The knowledge of the box model allows you to set the width and height of website elements correctly in al 

browsers.


Important: When you set the width and height properties of an element with CSS, you just set the width and 

height of the content area. To calculate the full size of an element, you must also add padding, borders and 

margins.


In the script below,

<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 320px;
  padding: 10px;
  border: 5px solid gray;
  margin: 0;
}
</style>
</head>
<body>

<h2>Calculate the total width:</h2>

<img src="klematis4_big.jpg" width="350" height="263" alt="Klematis">
<div>The picture above is 350px wide. The total width of this element is also 350px.</div>

</body>
</html>

The total width can be calculated as shown below,


320px (width)
+ 20px (left + right padding)
+ 10px (left + right border)
+ 0px (left + right margin)
= 350px 


The total width of an element should be calculated like this:

Total element width = width + left padding + right padding + left border + right border + left margin + 

right margin

Similarly, the total height of an element should be calculated as shown below:

Total element height = height + top padding + bottom padding + top border + bottom border + top margin + 

bottom margin

<kbd>return</kbd>[Back to table of contents](#homepage)


---------



## CSS Outline


Outline::

An outline is a line drawn around the elements (outside borders) to make the element "stand out"..

An outline can be created around an element using the script shown below:

<!DOCTYPE html>
<html>
<head>
<style>
p {
  border: 2px solid black;
  outline: #4CAF50 solid 2px;
  margin: auto;  
  padding: 20px;
  text-align: center;
}
</style>
</head>
<body>

<h2>CSS Outline</h2>
<p>This element has a 2px black border and a green outline with a width of 10px.</p>

</body>
</html>



The outline properties of CSS include,

    outline-style
    outline-color
    outline-width
    outline-offset
    outline


Note: Outline differs from borders! Unlike border, the outline is drawn outside the element's border, and 

may overlap other content. Also, the outline is NOT a part of the element's dimensions; the element's total 

width and height is not affected by the width of the outline.


CSS Outline Style

The outline-style property specifies the style of the outline, and can have one of the following values:

    dotted - Defines a dotted outline
    dashed - Defines a dashed outline
    solid - Defines a solid outline
    double - Defines a double outline
    groove - Defines a 3D grooved outline
    ridge - Defines a 3D ridged outline
    inset - Defines a 3D inset outline
    outset - Defines a 3D outset outline
    none - Defines no outline
    hidden - Defines a hidden outline


The implementation of the above outlines is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p {outline-color:red;}

p.dotted {outline-style: dotted;}
p.dashed {outline-style: dashed;}
p.solid {outline-style: solid;}
p.double {outline-style: double;}
p.groove {outline-style: groove;}
p.ridge {outline-style: ridge;}
p.inset {outline-style: inset;}
p.outset {outline-style: outset;}
</style>
</head>
<body>

<h2>The outline-style Property</h2>

<p class="dotted">A dotted outline</p>
<p class="dashed">A dashed outline</p>
<p class="solid">A solid outline</p>
<p class="double">A double outline</p>
<p class="groove">A groove outline. The effect depends on the outline-color value.</p>
<p class="ridge">A ridge outline. The effect depends on the outline-color value.</p>
<p class="inset">An inset outline. The effect depends on the outline-color value.</p>
<p class="outset">An outset outline. The effect depends on the outline-color value.</p>

</body>
</html>


NB: Note: None of the other outline properties (which you will learn more about in the next chapters) will 

have ANY effect unless the outline-style property is set!




CSS Outline Width

The width of the outline is specified using outline-width property, and this outline-width can have multiple 

values:



    thin (typically 1px)
    medium (typically 3px)
    thick (typically 5px)
    A specific size (in px, pt, cm, em, etc)

An example of how to specify outline-width is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: thin;
}

p.ex2 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: medium;
}

p.ex3 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: thick;
}

p.ex4 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: 4px;
}
</style>
</head>
<body>

<h2>The outline-width Property</h2>

<p class="ex1">A thin outline.</p>
<p class="ex2">A medium outline.</p>
<p class="ex3">A thick outline.</p>
<p class="ex4">A 4px thick outline.</p>

</body>
</html>




CSS Outline Color::


CSS Outline Color

The outline-color property is used to set the color of the outline.

The color can be set by:

    name - specify a color name, like "red"
    HEX - specify a hex value, like "#ff0000"
    RGB - specify a RGB value, like "rgb(255,0,0)"
    HSL - specify a HSL value, like "hsl(0, 100%, 50%)"
    invert - performs a color inversion (which ensures that the outline is visible, regardless of color 

background)


An example of the application of the outline-color property is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: red;
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: blue;
}

p.ex3 {
  border: 2px solid black;
  outline-style: outset;
  outline-color: grey;
}
</style>
</head>
<body>

<h2>The outline-color Property</h2>
<p>The outline-color property is used to set the color of the outline.</p>

<p class="ex1">A solid red outline.</p>
<p class="ex2">A dotted blue outline.</p>
<p class="ex3">An outset grey outline.</p>

</body>
</html>




HEX Values

The hexadecimal value can be used to specify the color of the outline as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: #ff0000; /* red */
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: #0000ff; /* blue */
}

p.ex3 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: #bbbbbb; /* grey */
}
</style>
</head>
<body>

<h2>The outline-color Property</h2>
<p>The color of the outline can also be specified using a hexadecimal value (HEX):</p>

<p class="ex1">A solid red outline.</p>
<p class="ex2">A dotted blue outline.</p>
<p class="ex3">A solid grey outline.</p>

</body>
</html>


RGB Values

The RGB values can also be used to specify the color of the outline as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: rgb(255, 0, 0); /* red */
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: rgb(0, 0, 255); /* blue */
}

p.ex3 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: rgb(187, 187, 187); /* grey */
}
</style>
</head>
<body>

<h2>The outline-color Property</h2>
<p>The color of the outline can also be specified using RGB values:</p>

<p class="ex1">A solid red outline.</p>
<p class="ex2">A dotted blue outline.</p>
<p class="ex3">A solid grey outline.</p>

</body>
</html>




HSL Values

The HSL values (hue, saturation, and lightness values) can also be used to specify the color of a CSS 

outline as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: hsl(0, 100%, 50%); /* red */
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: hsl(240, 100%, 50%); /* blue */
}

p.ex3 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: hsl(0, 0%, 73%); /* grey */
}
</style>
</head>
<body>

<h2>The outline-color Property</h2>
<p>The color of the outline can also be specified using HSL values:</p>

<p class="ex1">A solid red outline.</p>
<p class="ex2">A dotted blue outline.</p>
<p class="ex3">A solid grey outline.</p>

</body>
</html>





Invert Color

The outline-color: invert performs color inversion which enables visibility of the outline irrespective of 

the background color.

<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 1px solid yellow;
  outline-style: solid;
  outline-color: invert;
}
</style>
</head>
<body>

<h2>Using outline-color:invert</h2>

<p class="ex1">A solid invert outline.</p>

</body>
</html>


CSS Outline Shorthand::


CSS Outline - Shorthand property

The outline property is a shorthand property for setting the following individual outline properties:

    outline-width
    outline-style (required)
    outline-color

The outline property is specified as one, two, or three values from the list above. The order of the values 

does not matter.

The following example shows some outlines specified with the shorthand outline property:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {outline: dashed;}
p.ex2 {outline: dotted red;}
p.ex3 {outline: 5px solid yellow;}
p.ex4 {outline: thick ridge pink;}
</style>
</head>
<body>

<h2>The outline Property</h2>

<p class="ex1">A dashed outline.</p>
<p class="ex2">A dotted red outline.</p>
<p class="ex3">A 5px solid yellow outline.</p>
<p class="ex4">A thick ridge pink outline.</p>

</body>
</html>



CSS Outline Offset

The outline-offset property is used to include space between an outline and the edge/border of an element, 

leaving the space between an element and its outline transparent.


The script below shows how the outline offset is added to an element, such that the outline is 15px outside 

the border of the <p> element:


<!DOCTYPE html>
<html>
<head>
<style>
p {
  margin: 30px;
  border: 1px solid black;
  outline: 1px solid red;
  outline-offset: 15px;
}
</style>
</head>
<body>

<h2>The outline-offset Property</h2>

<p>This paragraph has an outline 15px outside the border edge.</p>

</body>
</html>



To visualize that the space between an element's border and its outline offset is transparent


<!DOCTYPE html>
<html>
<head>
<style>
p {
  margin: 30px;
  background:yellow;
  border: 1px solid black;
  outline: 1px solid red;
  outline-offset: 15px;
}
</style>
</head>
<body>

<h2>The outline-offset Property</h2>

<p>This paragraph has an outline of 15px outside the border edge.</p>

</body>
</html>



All CSS Outline Properties Summarized

All CSS Outline Properties
Property 	Description
outline 	A shorthand property for setting outline-width, outline-style, and outline-color in one 

declaration
outline-color 	Sets the color of an outline
outline-offset 	Specifies the space between an outline and the edge or border of an element
outline-style 	Sets the style of an outline
outline-width 	Sets the width of an outline


<kbd>return</kbd>[Back to table of contents](#homepage)



-----------


# CSS Text

We explain properties used in formatting texts in CSS under this section and subsections that follow.


Text formatting example is shown below:



<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid gray;
  padding: 8px;
}

h1 {
  text-align: center;
  text-transform: uppercase;
  color: #4CAF50;
}

p {
  text-indent: 50px;
  text-align: justify;
  letter-spacing: 3px;
}

a {
  text-decoration: none;
  color: #008CBA;
}
</style>
</head>
<body>

<div>
  <h1>text formatting</h1>
  <p>This text is styled with some of the text formatting properties. The heading uses the text-align, 

text-transform, and color properties.
  The paragraph is indented, aligned, and the space between characters is specified. The underline is 

removed from this colored
  <a target="_blank" href="tryit.asp?filename=trycss_text">"Try it Yourself"</a> link.</p>
</div>

</body>
</html>




Text Color::

The color property is used to set the color of the text using:


    a color name - like "red"
    a HEX value - like "#ff0000"
    an RGB value - like "rgb(255,0,0)"
NB: The default text color or a page is defined in the 'body' selector, under the <style> tags. See below 

for example:



<!DOCTYPE html>
<html>
<head>
<style>
body {
  color: blue;
}

h1 {
  color: green;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<p>This is an ordinary paragraph. Notice that this text is blue. The default text color for a page is 

defined in the body selector.</p>
<p>Another paragraph.</p>

</body>
</html>


Note: For W3C compliant CSS: If you define the color property, you must also define the background-color.



Text Color and Background Color

In this example, we define both the background-color property and the color property (for an element):


<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: lightgrey;
  color: blue;
}

h1 {
  background-color: black;
  color: white;
}
</style>
</head>
<body>

<h1>This Heading is Black with White Text</h1>
<p>This page has a grey background color and a blue text.</p>
<p>Another paragraph.</p>

</body>
</html>




CSS Text Alignment::

the css text-align property is used to set the horizontal alignment of a text to left, right, or justified 

aligned. If text direction is left-to-right, the default alignment is left. On the other hand, if the text 

is from right-to-left, the default alignment is right. An example of the use of text-align property is shown 

below:

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-align: center;
}

h2 {
  text-align: left;
}

h3 {
  text-align: right;
}
</style>
</head>
<body>

<h1>Heading 1 (center)</h1>
<h2>Heading 2 (left)</h2>
<h3>Heading 3 (right)</h3>

<p>The three headings above are aligned center, left and right.</p>

</body>
</html>


When the text-align property is set to "justify", each line is stretched so that every line has equal width, 

and the left and right margins are straight (like in magazines and newspapers):

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 10px;
  width: 200px;
  height: 200px;
  text-align: justify;
}
</style>
</head>
<body>

<h1>Example text-align: justify;</h1>

<p>The text-align: justify; value stretches the lines so that each line has equal width (like in newspapers 

and magazines).</p>

<div>
In my younger and more vulnerable years my father gave me some advice that I've been turning over in my mind 

ever since. 'Whenever you feel like criticizing anyone,' he told me, 'just remember that all the people in 

this world haven't had the advantages that you've had.'
</div>

</body>
</html>



Text Direction

The direction and unicode-bidi (invert each of the letters from left to right) properties can be used to 

change the text direction of an element:

<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  direction: rtl;
  unicode-bidi: bidi-override;
}
</style>
</head>
<body>

<p>This is the default text direction.</p>

<p class="ex1">This is right-to-left text direction.</p>

</body>
</html>


Vertical Alignment

The vertical-align property sets the vertical alignment of an element. The example below shows how to set 

the vertical alignment of an image in a text.



<!DOCTYPE html>
<html>
<head>
<style>
img.a {
  vertical-align: baseline;
}

img.b {
  vertical-align: text-top;
}

img.c {
  vertical-align: text-bottom;
}

img.d {
  vertical-align: sub;
}

img.e {
  vertical-align: super;
}
</style>
</head>
<body>

<h1>The vertical-align Property</h1>

<h2>vertical-align: baseline (default):</h2>
<p>An <img class="a" src="sqpurple.gif" width="9" height="9"> image with a default alignment.</p> 

<h2>vertical-align: text-top:</h2>
<p>An <img class="b" src="sqpurple.gif" width="9" height="9"> image with a text-top alignment.</p> 

<h2>vertical-align: text-bottom:</h2>
<p>An <img class="c" src="sqpurple.gif" width="9" height="9"> image with a text-bottom alignment.</p>

<h2>vertical-align: sub:</h2>
<p>An <img class="d" src="sqpurple.gif" width="9" height="9"> image with a sub alignment.</p> 

<h2>vertical-align: sup:</h2>
<p>An <img class="e" src="sqpurple.gif" width="9" height="9"> image with a super alignment.</p>

</body>
</html>



CSS Text Decoration


Text Decoration

The text-decoration property is used to set or remove decorations from text.

The value text-decoration: none; is often used to remove underlines from links:



<!DOCTYPE html>
<html>
<head>
<style>
a {
  text-decoration: none;
}
</style>
</head>
<body>

<p>A link with no underline: <a href="https://www.w3schools.com">W3Schools.com</a></p>

</body>
</html>




Other text decoration values are shown below:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-decoration: overline;
}

h2 {
  text-decoration: line-through;
}

h3 {
  text-decoration: underline;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>

</body>
</html>


Note: It is not recommended to underline text that is not a link, as this often confuses the reader.



Text Transformation::

The text-transform property is used to specify uppercase and lowercase letters in a text.

It can be used to turn everything into uppercase or lowercase letters, or capitalize the first letter of 

each word:



<!DOCTYPE html>
<html>
<head>
<style>
p.uppercase {
  text-transform: uppercase;
}

p.lowercase {
  text-transform: lowercase;
}

p.capitalize {
  text-transform: capitalize;
}
</style>
</head>
<body>

<p class="uppercase">This is some text.</p>
<p class="lowercase">This is some text.</p>
<p class="capitalize">This is some text.</p>

</body>
</html>






CSS Text Spacing::

The text-indent property is used to specify the indentation of the first line of a text.



<!DOCTYPE html>
<html>
<head>
<style>
p {
  text-indent: 50px;
}
</style>
</head>
<body>

<p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my 

mind ever since. 'Whenever you feel like criticizing anyone,' he told me, 'just remember that all the people 

in this world haven't had the advantages that you've had.'</p>

</body>
</html>



Letter Spacing

The letter-spacing property is used to specify the space between the characters in a text.

The following example demonstrates how to increase or decrease the space between characters:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  letter-spacing: 3px;
}

h2 {
  letter-spacing: -3px;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>

</body>
</html>




Line Height

The line-height property is used to specify the space between lines:


<!DOCTYPE html>
<html>
<head>
<style>
p.small {
  line-height: 0.7;
}

p.big {
  line-height: 1.8;
}
</style>
</head>
<body>

<p>
This is a paragraph with a standard line-height.<br>
The default line height in most browsers is about 110% to 120%.<br>
</p>

<p class="small">
This is a paragraph with a smaller line-height.<br>
This is a paragraph with a smaller line-height.<br>
</p>

<p class="big">
This is a paragraph with a bigger line-height.<br>
This is a paragraph with a bigger line-height.<br>
</p>

</body>
</html>















































Word Spacing

The word-spacing property is used to specify the space between the words in a text.

The following example demonstrates how to increase (positive value) or decrease (negative value) the space 

between words:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  word-spacing: 10px;
}

h2 {
  word-spacing: -5px;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>

</body>
</html>




White Space

The white-space property specifies how white-space inside an element is handled.

This example demonstrates how to disable text wrapping inside an element:



<!DOCTYPE html>
<html>
<head>
<style>
p {
  white-space: nowrap;
}
</style>
</head>
<body>

<h2>White Space</h2>

<p>
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
</p>

<p>Try to remove the white-space property to see the difference.</p>

</body>
</html>






CSS Text Shadow::


Text Shadow

The text-shadow property adds shadow to text.

In its simplest use, you only specify the horizontal shadow (2px) and the vertical shadow (2px):


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 2px 2px;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>




To add a color (red) to the shadow:

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 2px 2px red;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>




To add a blur effect (5px) to the shadow:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 2px 2px 5px red;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>


<kbd>return</kbd>[Back to table of contents](#homepage)


--------



## CSS Fonts


The right fond can improve UX of a website and can create a unique and strong brand identity. Readability of 

a font is very crucial, for font to add value to text. Color and text size of a font are important too while 

choosing a font.



Generic Font Families

In CSS there are five generic font families:

    Serif fonts have a small stroke at the edges of each letter. They create a sense of formality and 

elegance.
    Sans-serif fonts have clean lines (no small strokes attached). They create a modern and minimalistic 

look.
    Monospace fonts - here all the letters have the same fixed width. They create a mechanical look. 
    Cursive fonts imitate human handwriting.
    Fantasy fonts are decorative/playful fonts.

All the different font names belong to one of the generic font families. 



Note: On computer screens, sans-serif fonts are considered easier to read than serif fonts.


Some Font Examples

Generic Font Family    Examples of Font Names


Serif    		Times New Roman, Georgia, Garamond

Sans-serif		Arial Verdana, Helvetica

Monospace               Courier New, Lucida Console, Monaco,

Cursive			Brush Script MT, Lucida Handwriting

Fantasy			Copperplate, Papyrus



The CSS font-family Property

In CSS, we use the font-family property to specify the font of a text.

The font-family property should hold several font names as a "fallback" system, to ensure maximum 

compatibility between browsers/operating systems. Start with the font you want, and end with a generic 

family (to let the browser pick a similar font in the generic family, if no other fonts are available). The 

font names should be separated with comma.

Note: If the font name is more than one word, it must be in quotation marks, like: "Times New Roman". 

An example of the application of font-family in CSS is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
.p1 {
  font-family: "Times New Roman", Times, serif;
}

.p2 {
  font-family: Arial, Helvetica, sans-serif;
}

.p3 {
  font-family: "Lucida Console", "Courier New", monospace;
}
</style>
</head>
<body>

<h1>CSS font-family</h1>
<p class="p1">This is a paragraph, shown in the Times New Roman font.</p>
<p class="p2">This is a paragraph, shown in the Arial font.</p>
<p class="p3">This is a paragraph, shown in the Lucida Console font.</p>

</body>
</html>




CSS Web Safe Fonts::

They are fonts that are universally installed on all browsers and devices. 


Fallback Fonts: since there are no 100% web safe fonts, always use fallback fonts in case a font is not 

found or is not properly installed on the browser or device.


You should always add a list of similar 'backup fonts' in the font-family property.If the first font does 

not work, the browser will try the next one, and the next one, and so on. Always end the list with a generic 

font family name.



An illustration of this concept is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p {
font-family: Tahoma, Verdana, sans-serif;
}
</style>
</head>
<body>

<h1>CSS Fallback Fonts</h1>

<p>This is a paragraph.</p>
<p>This is another paragraph.</p>

</body>
</html>



Best Web Safe Fonts for HTML and CSS

The following list are the best web safe fonts for HTML and CSS:

    Arial (sans-serif)
    Verdana (sans-serif)
    Helvetica (sans-serif)
    Tahoma (sans-serif)
    Trebuchet MS (sans-serif)
    Times New Roman (serif)
    Georgia (serif)
    Garamond (serif)
    Courier New (monospace)
    Brush Script MT (cursive)

Note: Before you publish your website, always check how your fonts appear on different browsers and devices, 

and always use fallback fonts!


Arial (sans-serif)

Arial is the most widely used font for both online and printed media. Arial is also the default font in 

Google Docs.

Arial is one of the safest web fonts, and it is available on all major operating systems.

An example of specifying arial font with font-family 



<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Arial, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Verdana (sans-serif)

Verdana is a very popular font. Verdana is easily readable even for small font sizes.


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Verdana, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Helvetica (sans-serif)

The Helvetica font is loved by designers. It is suitable for many types of business. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Helvetica, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>




Tahoma (sans-serif)

The Tahoma font has less space between the characters. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Tahoma, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>


Trebuchet MS (sans-serif)

Trebuchet MS was designed by Microsoft in 1996. Use this font carefully. Not supported by all mobile 

operating systems. See example below:



<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: 'Trebuchet MS', sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Times New Roman (serif)

Times New Roman is one of the most recognizable fonts in the world. It looks professional and is used in 

many newspapers and "news" websites. It is also the primary font for Windows devices and applications. See 

example bnw


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: 'Times New Roman', serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Georgia (serif)

Georgia is an elegant serif font. It is very readable at different font sizes, so it is a good candidate for 

mobile-responsive design. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Georgia, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Garamond (serif)

Garamond is a classical font used for many printed books. It has a timeless look and good readability. See 

example below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Garamond, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Courier New (monospace)

Courier New is the most widely used monospace serif font. Courier New is often used with coding displays, 

and many email providers use it as their default font. Courier New is also the standard font for movie 

screenplays.



<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: 'Courier New', monospace;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>


Brush Script MT (cursive)

The Brush Script MT font was designed to mimic handwriting. It is elegant and sophisticated, but can be hard 

to read. Use it carefully. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: 'Brush Script MT', cursive;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



CSS Font Fallbacks::


Commonly Used Font Fallbacks

Below are some commonly used font fallbacks, organized by the 5 generic font families:

    Serif
    Sans-serif
    Monospace
    Cursive
    Fantasy

The different font families and the corresponding script to implement them are shown below:


Serif Fonts:::


font-family ("Times New Roman", Times, serif). see the code below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: "Times New Roman", Times, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Georgia, serif). See the code below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Georgia, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Garamond, serif). See the code to apply them below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Garamond, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>




Sans-Serif Fonts:::

font-family (Arial, Helvetica, san-serif). See the implementation below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Arial, Helvetica, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Tahoma, Verdana, sans-serif). See the implementation below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Tahoma, Verdana, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family ("Trebuchet MS", Helvetica, sans-serif). See the implementation below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: "Trebuchet MS", Helvetica, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Georgia, Verdana, sans-serif). See implementation below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Georgia, Verdana, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Monospace Fonts:::

font-family ("Courier New", Courier, monospace). See implementation below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: "Courier New", Courier, monospace;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Cursive Fonts:::

font-family ("Brush Script MT", cursive). See how to implement this font family below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: "Brush Script MT", cursive;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Fantasy Fonts:::

font-family (Copperplate, Papyrus, fantasy). See how to implement this font family below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Copperplate, Papyrus, fantasy;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>





CSS Font Style::


Font Style

The font-style property is mostly used to specify italic text.

This property has three values:

    normal - The text is shown normally
    italic - The text is shown in italics
    oblique - The text is "leaning" (oblique is very similar to italic, but less supported)


The implementation of font-style is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  font-style: normal;
}

p.italic {
  font-style: italic;
}

p.oblique {
  font-style: oblique;
}
</style>
</head>
<body>

<p class="normal">This is a paragraph in normal style.</p>
<p class="italic">This is a paragraph in italic style.</p>
<p class="oblique">This is a paragraph in oblique style.</p>

</body>
</html>




Font Weight

The font-weight property specifies the weight of a font:


<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  font-weight: normal;
}

p.light {
  font-weight: lighter;
}

p.thick {
  font-weight: bold;
}

p.thicker {
  font-weight: 900;
}
</style>
</head>
<body>

<p class="normal">This is a paragraph.</p>
<p class="light">This is a paragraph.</p>
<p class="thick">This is a paragraph.</p>
<p class="thicker">This is a paragraph.</p>

</body>
</html>


Font Variant

The font-variant property specifies whether or not a text should be displayed in a small-caps font.

In a small-caps font, all lowercase letters are converted to uppercase letters. However, the converted 

uppercase letters appears in a smaller font size than the original uppercase letters in the text.

<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  font-variant: normal;
}

p.small {
  font-variant: small-caps;
}
</style>
</head>
<body>

<p class="normal">My name is Hege Refsnes.</p>
<p class="small">My name is Hege Refsnes.</p>

</body>
</html>





CSS Font Size::



Font Size

The font-size property sets the size of the text.

Being able to manage the text size is important in web design. However, you should not use font size 

adjustments to make paragraphs look like headings, or headings look like paragraphs.

Always use the proper HTML tags, like <h1> - <h6> for headings and <p> for paragraphs.

The font-size value can be an absolute, or relative size.

Absolute size:

    Sets the text to a specified size
    Does not allow a user to change the text size in all browsers (bad for accessibility reasons)
    Absolute size is useful when the physical size of the output is known

Relative size:

    Sets the size relative to surrounding elements
    Allows a user to change the text size in browsers


Note: If you do not specify a font size, the default size for normal text, like paragraphs, is 16px 

(16px=1em).

Convertion factor: 1em=12pt=16px=100%



Set Font Size With Pixels

Setting the text size with pixels gives you full control over the text size:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  font-size: 40px;
}

h2 {
  font-size: 30px;
}

p {
  font-size: 14px;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>

</body>
</html>


Tip: If you use pixels, you can still use the zoom tool to resize the entire page.



Set Font Size With Em

To allow users to resize the text (in the browser menu), many developers use em instead of pixels.

1em is equal to the current font size. The default text size in browsers is 16px. So, the default size of 

1em is 16px.

The size can be calculated from pixels to em using this formula: pixels/16=em

See application below:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  font-size: 2.5em; /* 40px/16=2.5em */
}

h2 {
  font-size: 1.875em; /* 30px/16=1.875em */
 }

p {
  font-size: 0.875em; /* 14px/16=0.875em */
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<p>This is a paragraph.</p>
<p>Specifying the font-size in em allows all major browsers to resize the text.
Unfortunately, there is still a problem with older versions of IE. When resizing the text, it becomes 

larger/smaller than it should.</p>

</body>
</html>



In the example above, the text size in em is the same as the previous example in pixels. However, with the 

em size, it is possible to adjust the text size in all browsers.

Unfortunately, there is still a problem with older versions of Internet Explorer. The text becomes larger 

than it should when made larger, and smaller than it should when made smaller.




Use a Combination of Percent and Em

The solution that works in all browsers, is to set a default font-size in percent for the <body> element:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-size: 100%;
}

h1 {
  font-size: 2.5em;
}

h2 {
  font-size: 1.875em;
}

p {
  font-size: 0.875em;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<p>This is a paragraph.</p>
<p>Specifying the font-size in percent and em displays the same size in all major browsers, and allows all 

browsers to resize the text!</p>

</body>
</html>


NB: Our code now works great! It shows the same text size in all browsers, and allows all browsers to zoom 

or resize the text!



Responsive Font Size

The text size can be set with a vw unit, which means the "viewport width". Viewport is the browser window 

size. 1vw = 1% of viewport width. If the viewport is 50cm wide, 1vw is 0.5cm.

That way the text size will follow the size of the browser window:


<!DOCTYPE html>
<html>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<body>

<h1 style="font-size:10vw;">Responsive Text</h1>

<p style="font-size:5vw;">Resize the browser window to see how the text size scales.</p>

<p style="font-size:5vw;">Use the "vw" unit when sizing the text. 10vw will set the size to 10% of the 

viewport width.</p>

<p>Viewport is the browser window size. 1vw = 1% of viewport width. If the viewport is 50cm wide, 1vw is 

0.5cm.</p>

</body>
</html>





CSS Google Fonts::


Google fonts are 1000+ free-to-use additoinal fonts for people who prefer not to use the standard HTML 

fonts.

How To Use Google Fonts

Just add a special style sheet link in the <head> section and then refer to the font in the CSS.



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<style>
body {
  font-family: "Sofia", sans-serif;
}
</style>
</head>
<body>

<h1>Sofia Font</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>



To use a font named "Trirong" from Google Fonts:

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Trirong">
<style>
body {
  font-family: "Trirong", serif;
}
</style>
</head>
<body>

<h1>Trirong Font</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>


To use a font named "Audiowide" from Google Fonts:

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide">
<style>
body {
  font-family: "Audiowide", sans-serif;
}
</style>
</head>
<body>

<h1>Audiowide Font</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>




Note: When specifying a font in CSS, always list at minimum one fallback font (to avoid unexpected 

behaviors). So, also here you should add a generic font family (like serif or sans-serif) to the end of the 

list.

See all available google fonts here: https://www.w3schools.com/howto/howto_google_fonts.asp


To use multiple Google fonts, just separate the font names with a pipe character (|), like this:



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide|Sofia|Trirong">
<style>
h1.a {
  font-family: "Audiowide", sans-serif;
}

h1.b {
  font-family: "Sofia", sans-serif;
}

h1.c {
  font-family: "Trirong", serif;
}
</style>
</head>
<body>

<h1 class="a">Audiowide Font</h1>

<h1 class="b">Sofia Font</h1>

<h1 class="c">Trirong Font</h1>

</body>
</html>



NB: Requesting multiple fonts may slow down your web pages! So be careful about that.



Styling Google Fonts

CSS can be used to style Google Fonts as shown below:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
  text-shadow: 3px 3px 3px #ababab;
}
</style>
</head>
<body>

<h1>Sofia Font</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>




Enabling Font Effects

Google have also enabled different font effects that you can use.

First add effect=effectname to the Google API, then add a special class name to the element that is going to 

use the special effect. The class name always starts with font-effect- and ends with the effectname.


To add the fire effect to the "Sofia" font


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=fire">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
}
</style>
</head>
<body>

<h1 class="font-effect-fire">Sofia on Fire</h1>
<p class="font-effect-fire">Lorem ipsum dolor sit amet.</p>
<p class="font-effect-fire">123456790</p>

</body>
</html>


To request multiple font effects, just separate the effect names with a pipe character (|), like this:



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=neon|outline|emboss|

shadow-multiple">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
}
</style>
</head>
<body>

<h1 class="font-effect-neon">Neon Effect</h1>
<h1 class="font-effect-outline">Outline Effect</h1>
<h1 class="font-effect-emboss">Emboss Effect</h1>
<h1 class="font-effect-shadow-multiple">Multiple Shadow Effect</h1>

</body>
</html>





CSS Great Font Pairings::

It is important for a website to have great font pairings. This improves the design.


Font Pairing Rules

Here are some basic rules to create great font pairings:
1. Complement

It is always safe to find font pairings that complement one another.

A great font combination should harmonize, without being too similar or too different.
2. Use Font Superfamilies

A font superfamily is a set of fonts designed to work well together. So, using different fonts within the 

same superfamily is safe.

For example, the Lucida superfamily contains the following fonts: Lucida Sans, Lucida Serif, Lucida 

Typewriter Sans, Lucida Typewriter Serif and Lucida Math.
3. Contrast is King

Two fonts that are too similar will often conflict. However, contrasts, done the right way, brings out the 

best in each font.

Example: Combining serif with sans serif is a well known combination.

A strong superfamily includes both serif and sans serif variations of the same font (e.g. Lucida and Lucida 

Sans).
4. Choose Only One Boss

One font should be the boss. This establishes a hierarchy for the fonts on your page. This can be achieved 

by varying the size, weight and color.


In the example below, Georgia font family is the boss as it is larger and a compatible but different fonts:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: black;
  font-family: Verdana, sans-serif;
  font-size: 16px;
  color: gray;  
}

h1 {
  font-family: Georgia, serif;
  font-size: 60px;
  color: white;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html>




Some of the available popular font pairings that will suit many brands and contexts are shown in the 

examples below:


Georgia and Verdana

Georgia and Verdana is a classic combination. It also sticks to the web safe font standards. Use "Georgia" 

font for headings, and "Verdana" font for text. See example below:



<!DOCTYPE html>
<html>
<head>
<style>
body  {
  font-family: Verdana, sans-serif;
  font-size: 16px;
}

h1 {
  font-family: Georgia, serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Helvetica and Garamond

Helvetica and Garamond is another classic combination that uses web safe fonts. Use "Helvetica" font for 

headings and "Garamond" font for text. See example below:



<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Garamond, serif;
  font-size: 16px;  
}

h1 {
  font-family: Helvetica, sans-serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 





Popular Google Font Pairings

Google fonts provide 1000+ alternatives to traditional HTML fonts.They are free to use on your website. 


Below are the compatible google fonts




Merriweather and Open Sans 

Meriwether font for headings, and "Open Sans" for text::


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Merriweather|Open+Sans">
<style>
body {
  font-family: "Open Sans", sans-serif;
  font-size: 16px;
}

h1 {
  font-family: Merriweather, serif;
  font-size: 46px;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 




Ubuntu and Lora

USe Ubuntu for headings and Lora for text. See example below:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Ubuntu|Lora">
<style>
body {
  font-family: Lora, serif;
  font-size: 16px;  
}

h1 {
  font-family: Ubuntu, sans-serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Abril Fatface and Poppins

Use "Abril Fatface" font for headings, and "Poppins" for text. For example:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Abril+Fatface|Poppins">
<style>
body {
  font-family: Poppins, sans-serif;
  font-size: 16px;  
}

h1 {
  font-family: 'Abril Fatface', serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Cinzel and Fauna One

Use "Cinzel" font for headings and "Fauna One" for text.



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Cinzel|Fauna+One">
<style>
body {
  font-family: 'Fauna One', serif;
  font-size: 16px;  
}

h1 {
  font-family: Cinzel, serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Fjalla One and Libre Baskerville


The "Fjalla One" font should be used for headings and "Libre Baskerville" for text.


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Fjalla+One|Libre+Baskerville">
<style>
body {
  font-family: 'Libre Baskerville', serif;
  font-size: 16px;  
}

h1 {
  font-family: 'Fjalla One', sans-serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 




Space Mono and Muli

Use "Space Mono" font for headings, and "Muli" for text. See example below:



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Space+Mono|Muli">
<style>
body {
  font-family: Muli, sans-serif;
  font-size: 16px;
}

h1 {
  font-family: "Space Mono", monospace;
  font-size: 46px;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Spectral and Rubik

Use the Spectral font for headings and "Rubik" for text:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Spectral|Rubik">
<style>
body {
  font-family: Rubik, sans-serif;
  font-size: 16px;
}

h1 {
  font-family: Spectral, serif;
  font-size: 46px;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 





Oswald and Noto Sans

Use the "Oswald" font for headings and "Noto Sans" for text. See an example below:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Oswald|Noto+Sans">
<style>
body {
  font-family: "Noto Sans", sans-serif;
  font-size: 16px;
}

h1 {
  font-family: Oswald, sans-serif;
  font-size: 46px;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 




CSS Font Property::


To shorten the code, it is also possible to specify all the individual font properties in one property.

The font property is a shorthand property for:

    font-style
    font-variant
    font-weight
    font-size/line-height
    font-family

See an example of this application below:

<!DOCTYPE html>
<html>
<head>
<style>
p.a {
  font: 20px Arial, sans-serif;
}

p.b {
  font: italic bold 12px/30px Georgia, serif;
}
</style>
</head>
<body>

<h1>The font Property</h1>

<p class="a">This is a paragraph. The font size is set to 20 pixels, and the font family is Arial.</p>

<p class="b">This is a paragraph. The font is set to italic and bold, the font size is set to 12 pixels, the 

line height is set to 30 pixels, and the font family is Georgia.</p>

</body>
</html>


Note: The font-size and font-family values are required. If one of the other values is missing, their 

default value are used.

<kbd>return</kbd>[Back to table of contents](#homepage)
 - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  - - -  - - - - - - - - - - - - - - - - - -- - - - - - -- - - -


## CSS Icons

There is an icon library in CSS that facilitates the addition of icons to an HTML page. 


How to Add Icons

Icon can be simply added to an HTML page with an icon library like Font Awesome. You simply add the name of 

the specified icon class to any inline HTML element (like <i> or <span>). The resulting icons are scalable 

vectors that you can customize using the CSS styling tools to change the size, color, shadow, etc of such 

icons.

 

Font Awesome Icons

Go to fontawesome.com and sign in. The code needed to be added to the <head> section of the HTML page can be 

obtained on this website as shown below:

<script src="https://kit.fontawesome.com/yourcode.js" crossorigin="anonymous"></script>


To learn more about how to get started in font-awesome, check here: 

https://www.w3schools.com/icons/fontawesome5_intro.asp

YOu do not need any downloading or installation to use font awesome


A full list of references of all icons available in font awesome can be see here: 

https://www.w3schools.com/icons/icons_reference.asp


An example of implementation of font awesome is shown below:


<!DOCTYPE html>
<html>
<head>
<title>Font Awesome Icons</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
<!--Get your own code at fontawesome.com-->
</head>
<body>

<p>Some Font Awesome icons:</p>
<i class="fas fa-cloud"></i>
<i class="fas fa-heart"></i>
<i class="fas fa-car"></i>
<i class="fas fa-file"></i>
<i class="fas fa-bars"></i>

<p>Styled Font Awesome icons (size and color):</p>
<i class="fas fa-cloud" style="font-size:24px;"></i>
<i class="fas fa-cloud" style="font-size:36px;"></i>
<i class="fas fa-cloud" style="font-size:48px;color:red;"></i>
<i class="fas fa-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>




Bootstrap Icons

To use the Bootstrap glyphicons, add the following line inside the <head> section of your HTML page:

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">

Note: No downloading or installation is required!


See example of the implementation of Boostrap icon below:

<!DOCTYPE html>
<html>
<head>
<title>Bootstrap Icons</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
</head>
<body class="container">

<p>Some Bootstrap icons:</p>
<i class="glyphicon glyphicon-cloud"></i>
<i class="glyphicon glyphicon-remove"></i>
<i class="glyphicon glyphicon-user"></i>
<i class="glyphicon glyphicon-envelope"></i>
<i class="glyphicon glyphicon-thumbs-up"></i>
<br><br>

<p>Styled Bootstrap icons (size and color):</p>
<i class="glyphicon glyphicon-cloud" style="font-size:24px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:36px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:48px;color:red;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>



Google Icons

To use the Google icons, add the following line inside the <head> section of your HTML page:

<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">

Note: No downloading or installation is required!

See the example of the implementation of google icon below:



<!DOCTYPE html>
<html>
<head>
<title>Google Icons</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
</head>
<body>

<p>Some Google icons:</p>
<i class="material-icons">cloud</i>
<i class="material-icons">favorite</i>
<i class="material-icons">attachment</i>
<i class="material-icons">computer</i>
<i class="material-icons">traffic</i>
<br><br>

<p>Styled Google icons (size and color):</p>
<i class="material-icons" style="font-size:24px;">cloud</i>
<i class="material-icons" style="font-size:36px;">cloud</i>
<i class="material-icons" style="font-size:48px;color:red;">cloud</i>
<i class="material-icons" style="font-size:60px;color:lightblue;">cloud</i>

</body>
</html>


<kbd>return</kbd>[Back to table of contents](#homepage)


--------

## CSS Icons

There is an icon library in CSS that facilitates the addition of icons to an HTML page. 


How to Add Icons

Icon can be simply added to an HTML page with an icon library like Font Awesome. You simply add the name of 

the specified icon class to any inline HTML element (like <i> or <span>). The resulting icons are scalable 

vectors that you can customize using the CSS styling tools to change the size, color, shadow, etc of such 

icons.

 

Font Awesome Icons

Go to fontawesome.com and sign in. The code needed to be added to the <head> section of the HTML page can be 

obtained on this website as shown below:

<script src="https://kit.fontawesome.com/yourcode.js" crossorigin="anonymous"></script>


To learn more about how to get started in font-awesome, check here: 

https://www.w3schools.com/icons/fontawesome5_intro.asp

YOu do not need any downloading or installation to use font awesome


A full list of references of all icons available in font awesome can be see here: 

https://www.w3schools.com/icons/icons_reference.asp


An example of implementation of font awesome is shown below:


<!DOCTYPE html>
<html>
<head>
<title>Font Awesome Icons</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
<!--Get your own code at fontawesome.com-->
</head>
<body>

<p>Some Font Awesome icons:</p>
<i class="fas fa-cloud"></i>
<i class="fas fa-heart"></i>
<i class="fas fa-car"></i>
<i class="fas fa-file"></i>
<i class="fas fa-bars"></i>

<p>Styled Font Awesome icons (size and color):</p>
<i class="fas fa-cloud" style="font-size:24px;"></i>
<i class="fas fa-cloud" style="font-size:36px;"></i>
<i class="fas fa-cloud" style="font-size:48px;color:red;"></i>
<i class="fas fa-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>




Bootstrap Icons

To use the Bootstrap glyphicons, add the following line inside the <head> section of your HTML page:

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">

Note: No downloading or installation is required!


See example of the implementation of Boostrap icon below:

<!DOCTYPE html>
<html>
<head>
<title>Bootstrap Icons</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
</head>
<body class="container">

<p>Some Bootstrap icons:</p>
<i class="glyphicon glyphicon-cloud"></i>
<i class="glyphicon glyphicon-remove"></i>
<i class="glyphicon glyphicon-user"></i>
<i class="glyphicon glyphicon-envelope"></i>
<i class="glyphicon glyphicon-thumbs-up"></i>
<br><br>

<p>Styled Bootstrap icons (size and color):</p>
<i class="glyphicon glyphicon-cloud" style="font-size:24px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:36px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:48px;color:red;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>



Google Icons

To use the Google icons, add the following line inside the <head> section of your HTML page:

<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">

Note: No downloading or installation is required!

See the example of the implementation of google icon below:



<!DOCTYPE html>
<html>
<head>
<title>Google Icons</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
</head>
<body>

<p>Some Google icons:</p>
<i class="material-icons">cloud</i>
<i class="material-icons">favorite</i>
<i class="material-icons">attachment</i>
<i class="material-icons">computer</i>
<i class="material-icons">traffic</i>
<br><br>

<p>Styled Google icons (size and color):</p>
<i class="material-icons" style="font-size:24px;">cloud</i>
<i class="material-icons" style="font-size:36px;">cloud</i>
<i class="material-icons" style="font-size:48px;color:red;">cloud</i>
<i class="material-icons" style="font-size:60px;color:lightblue;">cloud</i>

</body>
</html>


<kbd>return</kbd>[Back to table of contents](#homepage)



---------

## HTML TABLES
```
<table> tag defined the HTML table. 
<tr> defines table row
<th> defines table header. By default bold and centered.
<td> defines table data/cell.. By default regular and left-aligned. They are data containers for text, images, lists, other tables, etc.
```
* A Simple HTML Table
```
 <table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table> 
```
** Table looks like this::
Firstname 	Lastname 	Age
Jill 	Smith 	50
Eve 	Jackson 	94
John 	Doe 	80


* Add a border to HTML table:::
```
table, th, td {
  border: 1px solid black;
}
```

** Collapsed Table Border:: Add Border collapse property to enable all borders to collapse into  one border. 
```
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
```

** Add Cell Padding::: Specifies the space between the cell and its borders. If not specified, table cells are displayed without padding. Use css padding property to set padding:

```
th, td {
  padding: 15px;
}
```
** Left-align Headings::Table headings are by default bold and centred. 

To left-align table headings, use CSS text-align property. 
```
th {
  text-align: left;
}
```

** Add border spacing:: Specifies space between cells. Use CSS border-spacing property. Border spacing has no effect for table with collapsed borders
```
table {
  border-spacing: 5px;
}
```
** Cells that Spans Many Columns:: use colspan attribute
```
 <table style="width:100%">
  <tr>
    <th>Name</th>
    <th colspan="2">Telephone</th>
  </tr>
  <tr>
    <td>Bill Gates</td>
    <td>55577854</td>
    <td>55577855</td>
  </tr>
</table> 
```

** Looks like this:Name 	Telephone
Bill Gates 	55577854 	55577855


** Make cell that spans many rows::use rowspan. rowspan=2 means that you will specify two row <tr> elements to contain the content spanning two rows
	
```
 <table style="width:100%">
  <tr>
    <th>Name:</th>
    <td>Bill Gates</td>
  </tr>
  <tr>
    <th rowspan="2">Telephone:</th>
    <td>55577854</td>
  </tr>
  <tr>
    <td>55577855</td>
  </tr>
</table> 
```
** Add a caption to the table:: use <caption>  tag...inserted immediately after the table tag
	
```
 <table style="width:100%">
  <caption>Monthly savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$50</td>
  </tr>
</table> 
```
** Define a special style for one table. Add an id to the table and then define the special style next
``` 
<table id="t01">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table> 


#t01 {
  width: 100%;
  background-color: #f1f1c1;
}

```

you can also add more styles:
```
#t01 tr:nth-child(even) {
  background-color: #eee;
}
#t01 tr:nth-child(odd) {
  background-color: #fff;
}
#t01 th {
  color: white;
  background-color: black;
}
```


* CHAPTER SUMMARY _HTML CHAPTER SUMMARY
   Use the HTML ```<table>``` element to define a table
   Use the HTML ``<tr>``element to define a table row
   Use the HTML ``<td>`` element to define a table data
   Use the HTML ```<th>``` element to define a table heading
   Use the HTML ```<caption>``` element to define a table caption
   Use the CSS border property to define a border
   Use the CSS border-collapse property to collapse cell borders
   Use the CSS padding property to add padding to cells
   Use the CSS text-align property to align cell text
   Use the CSS border-spacing property to set the spacing between cells
   Use the colspan attribute to make a cell span many columns
   Use the rowspan attribute to make a cell span many rows
   Use the id attribute to uniquely define one table


<kbd>return</kbd>[Back to table of contents](#homepage)

--------



# HTML LISTS

** unordered list has bullets
** ordered lists have numberings or some kind of sequence labels

* Unordered html list:: each starts with ```<ul>``` tag and each list item starts with ```<li>``` tag
by default, list item  is marked with small black circles as bullets.
```
 <ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul> 
```

<kbd>return</kbd>[Back to table of contents](#homepage)

## ORDERED

* Ordered HTML list: Marked by <ol> and each list item is marked by <li> tag. Numbers are usd to mark list items by default.

```
 <ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol> 
```

HTML Description lists:: List of terms with description of each term in the list. description list is marked by ```<dl>``` tag and each description term (name) is marked by ```<dt>``` xyz and the description of each description list term is tagged by ```<dd>```:
```
 <dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl> 
```

* HTML List tags summary
Tag 	Description
```<ul>``` 	Defines an unordered list
```<ol>``` 	Defines an ordered list
```<li>``` 	Defines a list item
```<dl>``` 	Defines a description list
```<dt>``` 	Defines a term in a description list
```<dd>``` 	Describes the term in a description list

<kbd>return</kbd>[Back to table of contents](#homepage)

## UNORDERED
**HTML Unordered lists cont'd-List marker

To choose list marker, use css list-style-type property to define style of the list item market.

Value 	Description
disc 	Sets the list item marker to a bullet (default)
circle 	Sets the list item marker to a circle
square 	Sets the list item marker to a square
none 	The list items will not be marked

* Disc(filled circle)
```
<ul style="list-style-type:disc;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul> 
```

* Open( unfilled circle)
```
 <ul style="list-style-type:circle;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul> 
```

** Square (filled with black)
```
 <ul style="list-style-type:square;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul> 
```

** None ( No marker)
```
 <ul style="list-style-type:none;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul> 
```

** Nested HTML List: List inside list
```
 <ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul> 
```
** A list item (```<li>```) can contain a new list, and other HTML elements, like images and links, etc.

* Horizontal list with CSS

You can style lists horizontally, to create a navigation menu. 

** You can style list horizontally to create a navigation menu. The float style left sets the navigation menu to the left
```
 <!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111111;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html> 
```

** Chapter Summary
Chapter Summary

 Use the HTML ```<ul>``` element to define an unordered list
 Use the CSS list-style-type property to define the list item marker
 Use the HTML ```<li>``` element to define a list item
 Lists can be nested
 List items can contain other HTML elements
 Use the CSS property float:left to display a list horizontally

** HTML List Tags Summary
```
HTML List Tags
Tag 	Description
<ul> 	Defines an unordered list
<ol> 	Defines an ordered list
<li> 	Defines a list item
<dl> 	Defines a description list
<dt> 	Defines a term in a description list
<dd> 	Describes the term in a description list
```
<kbd>return</kbd>[Back to table of contents](#homepage)

HTML Ordered List:: 
```<ol>``` tag defines an ordered list which can be numerical or alphabetical.
List are marked by numbers by default

** Ordered HTML List - The Type Attribute
With the type attribute of the <ol> tag, you can define the type of the list item marker

```
Type 	Description
type="1" 	The list items will be numbered with numbers (default)
type="A" 	The list items will be numbered with uppercase letters
type="a" 	The list items will be numbered with lowercase letters
type="I" 	The list items will be numbered with uppercase roman numbers
type="i" 	The list items will be numbered with lowercase roman numbers
```


* Numbers
```
 <ol type="1">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol> 
```


* Uppercase Letters:
```
 <ol type="A">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol> 
```

* Lowercase Letters:
```
 <ol type="a">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol> 
```

* Uppercase Roman Numbers:
```
<ol type="I">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol> 
```
* Lowercase Roman Numbers:
```
<ol type="I">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol> 
```
* Control List Counting: Enables you to be able to start counting controlled list at a certain number other than 50
```
<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol> 
```
<kbd>return</kbd>[Back to table of contents](#homepage)

## OTHER
* Nested HTML Lists(list inside list)
```
<ol>
  <li>Coffee</li>
  <li>Tea
    <ol>
      <li>Black tea</li>
      <li>Green tea</li>
    </ol>
  </li>
  <li>Milk</li>
</ol> 
```
* Chapter summary:

Use the HTML ```<ol>``` element to define an ordered list
Use the HTML type attribute to define the numbering type
Use the HTML ```<li>``` element to define a list item
Lists can be nested
List items can contain other HTML elements

HTML List Tags
```
<ul> 	Defines an unordered list
<ol> 	Defines an ordered list
<li> 	Defines a list item
<dl> 	Defines a description list
<dt> 	Defines a term in a description list
<dd> 	Describes the term in a description list
```

* Description lists: List of terms with a description of each term. 
```<dl>``` tag defines the list, ```<dt>``` defines the term (name), and ```<dd>``` tag describes each term:
```
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl> 
```
* Description list summary:
Use the HTML ```<dl>``` element to define a description list
Use the HTML ```<dt>``` element to define the description term
Use the HTML ```<dd>``` element to describe the term in a description list

HTML List Tags
```
**Tag 	Description
<ul> 	Defines an unordered list
<ol> 	Defines an ordered list
<li> 	Defines a list item
<dl> 	Defines a description list
<dt> 	Defines a term in a description list
<dd> 	Describes the term in a description list
```
<kbd>return</kbd>[Back to table of contents](#homepage)


