## HTML FORMATTING
```
<b> - Bold text
<strong> - Important text
<i> - Italic text...often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc.
<em> - Emphasized text. A screen reader will emphasize the text using verbal stress
<mark> - Marked text. Element that should be highlighted. You can use style to change the color.
<small> - Smaller text
<del> - Deleted text. Browsers usually strike a line through
<ins> - Inserted text... (into a document) Browsers usually underline this. Can be used after del. 
<sub> - Subscript text...appears half a character below the normal line
<sup> - Superscript text...can be used for footnotes citation
```
```
*<p>My favorite color is <del>blue</del> <ins>red</ins>.</p>
```
<kbd>return</kbd>[Back to table of contents](#homepage)


--------------


## HTML QUOTATIONS
HTML QUOTATIONs AND CITATION ELEMENTS
```
<abbr> 	Defines an abbreviation or acronym. Marking them give information to browsers, translation systems and search engines. Use global attribute title with it to show full meaning of the abbreviation.
<address> 	Defines contact information for the author/owner of a document or an article. This can be email, url, physical, mobile no, social media handles etc. Browsers add line break before and after <address> element.
<bdo> 	Defines the text direction.Used to override current text direction
<blockquote>	Defines a section that is quoted from another source. Browser usually indents this. cite is used here to show the source, not href.
<cite> 	Defines the title of a creative work. Creator's name is not a title.Browsers will usually cite this element in italic
<q> 	Defines a short inline quotation.Browser inserts quotation marks around the quotation
```
* Quote
```
 <p>Here is a quote from WWF's website:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature.
The world's leading conservation organization,
WWF works in 100 countries and is supported by
1.2 million members in the United States and
close to 5 million globally.
</blockquote> 
```
* Short Quotations
```
 <p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p> 
```
* The use of abbreviation ```<abbr>```
```
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p> 
```
Address
```
<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address> 
```
* Cite for work title
 ```
 <p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p> 
```
* Bi-Directional Override(BDO)
```
 <bdo dir="rtl">This text will be written from right to left</bdo> 
```
<kbd>return</kbd>[Back to table of contents](#homepage)

--------


## HTML COMMENTS
There is only exclamation at the start not at the end
```
<!-- Write your comments here -->
```
Example usage
```
<!-- This is a comment -->

<p>This is a paragraph.</p>

<!-- Remember to add more information here -->
```
* Comments can help you to debug your html lines of code
<kbd>return</kbd>[Back to table of contents](#homepage)



---------------

## HTML COLORS
You specify them with color names, RGB, HEX, HSL,RGBA(the alpha is for transparency),HSLA values.
HTML supports 140 standard color names
* Specify background color as shown below:
```
<h1 style="background-color:DodgerBlue;">Hello World</h1>
<p style="background-color:Tomato;">Lorem ipsum...</p> 
```
* Set color of text 
```
<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Ut wisi enim...</p> 
```
* Set Color of border ( the square box) around text
```
<h1 style="border:2px solid Tomato;">Hello World</h1>
<h1 style="border:2px solid DodgerBlue;">Hello World</h1>
<h1 style="border:2px solid Violet;">Hello World</h1> 
```
## RGB
* These are all the same
```
rgb(255, 99, 71)
#ff6347
hsl(9, 100%, 64%)
```
* RGBA, HSLA
```
rgba(255, 99, 71, 0.5)
hsla(9, 100%, 64%, 0.5)
```
```
<h1 style="background-color:rgb(255, 99, 71);">...</h1>
<h1 style="background-color:#ff6347;">...</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>

<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1> 
```
<kbd>return</kbd>[Back to table of contents](#homepage)
## RGBA
RGB and RGBA Coloring
Red, Green, Blue, and Alpha
```rgb(r,g,b)```  each parameter has a value between  0 and 255 i.e 256 in total
Total number of colors: 256 x 256 x 256 = 16777216 possible colors!
```
Red color: rgb(255, 0, 0), 
Green color: rgb(0, 255, 0)
Black: rgb(0, 0, 0)
White:rgb(255, 255, 255). 
Grey: rgb( x,x,x) where x is not zero or 255. Black and white are at the two ends of the color spectrum.
```
RGBA
```rgba(red, green, blue, alpha)``` alpha 0 means fully transparent while 1.0 is not transparent at all. 
<kbd>return</kbd>[Back to table of contents](#homepage)
HTML HEX COLORS
RR(RED), GG(GREEN)BB(BLUE)...HEXADECIMAL INTEGERS SPECIFY THE COMPONENTS OF THE COLORS, EACH WITH VALUES RANGING FROM 00 TO ff ( same as decimal 0-255)
```#ff0000```- red since red has the highest value (ff) while the green and blue appear as 00 and 00
```#00ff00``` appears as green since green is set to the highest value(ff) and the remaining two have zero values
To display black, set all color parameters to 00, like this: ```#000000```.
To display white, setll all color parameters to ff: ```#ffffff```
Shades of gray: Equal values for all the parameters:
Each one of these are different shades of gray.
```
#404040
#686868
#a0a0a0
```
<kbd>return</kbd>[Back to table of contents](#homepage)
## HSL AND HSLA
HSL: Hue, Saturation, and, lightness
HSLA: Hue, Saturation, Lightness, and Alpha.
Hue: Degree on the colorwheel from 0 to 360  0 is red, 120 gree, 240 blue
Saturation: It is a percentage value. 0% is black, and 100 % is full color 
Lightness:Alsp a percentage value: 0% is black and 100% white
Saturation can be described as the intensity of a color. It is about how much shade of gray you want to have showing up on the color. 
100% is pure color, no shades of gray
50% is 50% gray, but you can still see the color.
0% is completely gray, you can no longer see the color.
** The lightness of a color can be described as how much light you want to give the color, where 0% means no light (black), 50% means 50% light (neither dark nor light) 100% means full lightness (white).
Shades of Gray: Can be obtained by setting hue and saturation to 0, and adjust the lighness from 0 % to 100 % to get darker/lighter shades: 
```
hsl(0, 0%, 20%)   --darker shade of grey
hsl(0, 0%, 70%)== lighter shade of grey
```
HSLA Color Values: 
Alpha rep transparency. 0.00 means fully transparent and 1.0 not transparent at all. 
<kbd>return</kbd>[Back to table of contents](#homepage)


---------



## HTML CSS
HTML STYLES-CSS
CSS can control layout of multiple pages at same time. 
CSS: CAscading style sheets: To control color, font, the size of text, the spacing between elements, how elements are positioned and laid out, what background images or background colors are to be used, different displays for different devices and screen sizes etc
Tip: The word cascading means that a style applied to a parent element will also apply to all children elements within the parent. So, if you set the color of the body text to "blue", all headings, paragraphs, and other text elements within the body will also get the same color (unless you specify something else)!
CSS can be added to HTML documents in 3 ways:
   Inline - by using the style attribute inside HTML elements
   Internal - by using a ```<style>``` element in the ```<head>``` section
   External - by using a ```<link>``` element to link to an external CSS file
	
<kbd>return</kbd>[Back to table of contents](#homepage)
## CSS INLINE
Inline CSS: To apply a unique style to a single HTML element, and it uses the style attribute of such element. 
* Set h1 color to blue and p to red
```
<h1 style="color:blue;">A Blue Heading</h1>

<p style="color:red;">A red paragraph.</p> 
```
<kbd>return</kbd>[Back to table of contents](#homepage)
# CSS INTERNAL
Internal CSS: To define style for a single HTML Page and it defined in <head> section of an html page within <style> element
```
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html> 
```
<kbd>return</kbd>[Back to table of contents](#homepage)


--------  

## CSS INTRODUCTION


CSS Solved a Big problem:
HTML was NEVER intended to contain tags for formatting a web page!

HTML was created to describe the content of a web page, like:

```
<h1>This is a heading</h1>

<p>This is a paragraph.</p>
```
  
Adding fonts color to HTML elements which was introduced in html 3 was a deviation from what HTML was meant 

to do in the first place.

CSS Saves a Lot of Work!

The style definitions are normally saved in external .css files.

With an external stylesheet file, you can change the look of an entire website by changing just one file!


<kbd>return</kbd>[Back to table of contents](#homepage)


--------- 

## CSS SYNTAX

```
h1 {color:blue;font-size:12px;}

selector {property:value;property:value;} 
```
property+value=declaration block.

  
```
p {
  color: red;
  text-align: center;
} 

```

the p is set to red and centered automatically.


<kbd>return</kbd>[Back to table of contents](#homepage)


------



## CSS SELECTORS

They help in dictating the styles of specific html elements

Categories of css selectors::

Simple selectors: use name, id, and class to select elements
Combinator selectors: use relationship between elements to select them
Pseudo-class selectors: To select elements based on a certain state
Pseudo-elements selectors:select and style part of an element
Attribute selectors: Use an attribute or attribute value to select an element

Explaining the most basic css selectors

1. CSS element Selector: Uses element name to select html elements

```
p {
  text-align: center;
  color: red;
}

```


2. CSS id Selector: Uses the id attribute of an element to select it. Element id is unique within a webpage 

and it can select one unique element. 
To use id to select element, use hash(#) followed by the id of the element.The name of an id cannot start 

with a number.

```
<!DOCTYPE html>
<html>
<head>
<style>
#para1 {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<p id="para1">Hello World!</p>
<p>This paragraph is not affected by the style.</p>

</body>
</html>

```



The CSS class Selector: Selects html elements with specific class attribute. Use (.) character followed by 

class name. The code below makes class="center" red and center-aligned

```

<!DOCTYPE html>
<html>
<head>
<style>
.center {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<h1 class="center">Red and center-aligned heading</h1>
<p class="center">Red and center-aligned paragraph.</p> 

</body>
</html>

```


You can also specify only html elements that should be affected by a class styling. In the code below, only 

```p``` elements with ```class="center"``` will be red and center aligned.

```

<!DOCTYPE html>
<html>
<head>
<style>
p.center {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<h1 class="center">This heading will not be affected</h1>
<p class="center">This paragraph will be red and center-aligned.</p> 

</body>
</html>

```

HTMl elements can refer to more than one class. In that case, p elemen is styled according to all the 

classes


```
<!DOCTYPE html>
<html>
<head>
<style>
p.center {
  text-align: center;
  color: red;
}

p.large {
  font-size: 300%;
}
</style>
</head>
<body>

<h1 class="center">This heading will not be affected</h1>
<p class="center">This paragraph will be red and center-aligned.</p>
<p class="center large">This paragraph will be red, center-aligned, and in a large font-size.</p> 

</body>
</html>
```


The CSS Universal Selector

The * selects all the HTML elements on a page

```
<!DOCTYPE html>
<html>
<head>
<style>
* {
  text-align: center;
  color: blue;
}
</style>
</head>
<body>

<h1>Hello world!</h1>

<p>Every element on the page will be affected by the style.</p>
<p id="para1">Me too!</p>
<p>And me!</p>

</body>
</html>

```


The CSS Grouping Selector::

Selects all the html elements with same sty le definitions. 


rather than having the code below:

```
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

We can simply have:

```

h1, h2, p {
  text-align: center;
  color: red;
}

```
and still get the same result


Summary of all CSS selectors:

All CSS Simple Selectors
  
```
Selector 	Example 	Example description

#id 	#firstname 	Selects the element with id="firstname"
.class 	.intro 	Selects all elements with class="intro"
element.class 	p.intro 	Selects only <p> elements with class="intro"
* 	* 	Selects all elements
element 	p 	Selects all <p> elements
element,element,.. 	div, p 	Selects all <div> elements and all <p> elements
```



<kbd>return</kbd>[Back to table of contents](#homepage)

---------


## CSS SELECTORS

They help in dictating the styles of specific html elements

Categories of css selectors::

Simple selectors: use name, id, and class to select elements
Combinator selectors: use relationship between elements to select them
Pseudo-class selectors: To select elements based on a certain state
Pseudo-elements selectors:select and style part of an element
Attribute selectors: Use an attribute or attribute value to select an element

Explaining the most basic css selectors

1. CSS element Selector: Uses element name to select html elements

```
p {
  text-align: center;
  color: red;
}

```


2. CSS id Selector: Uses the id attribute of an element to select it. Element id is unique within a webpage 

and it can select one unique element. 
To use id to select element, use hash(#) followed by the id of the element.The name of an id cannot start 

with a number.

```
<!DOCTYPE html>
<html>
<head>
<style>
#para1 {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<p id="para1">Hello World!</p>
<p>This paragraph is not affected by the style.</p>

</body>
</html>

```



The CSS class Selector: Selects html elements with specific class attribute. Use (.) character followed by 

class name. The code below makes class="center" red and center-aligned

```

<!DOCTYPE html>
<html>
<head>
<style>
.center {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<h1 class="center">Red and center-aligned heading</h1>
<p class="center">Red and center-aligned paragraph.</p> 

</body>
</html>

```


You can also specify only html elements that should be affected by a class styling. In the code below, only 

```p``` elements with ```class="center"``` will be red and center aligned.

```

<!DOCTYPE html>
<html>
<head>
<style>
p.center {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<h1 class="center">This heading will not be affected</h1>
<p class="center">This paragraph will be red and center-aligned.</p> 

</body>
</html>

```

HTMl elements can refer to more than one class. In that case, p elemen is styled according to all the 

classes


```
<!DOCTYPE html>
<html>
<head>
<style>
p.center {
  text-align: center;
  color: red;
}

p.large {
  font-size: 300%;
}
</style>
</head>
<body>

<h1 class="center">This heading will not be affected</h1>
<p class="center">This paragraph will be red and center-aligned.</p>
<p class="center large">This paragraph will be red, center-aligned, and in a large font-size.</p> 

</body>
</html>
```


The CSS Universal Selector

The * selects all the HTML elements on a page

```
<!DOCTYPE html>
<html>
<head>
<style>
* {
  text-align: center;
  color: blue;
}
</style>
</head>
<body>

<h1>Hello world!</h1>

<p>Every element on the page will be affected by the style.</p>
<p id="para1">Me too!</p>
<p>And me!</p>

</body>
</html>

```


The CSS Grouping Selector::

Selects all the html elements with same sty le definitions. 


rather than having the code below:

```
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

We can simply have:

```

h1, h2, p {
  text-align: center;
  color: red;
}

```
and still get the same result


Summary of all CSS selectors:

All CSS Simple Selectors
  
```
Selector 	Example 	Example description

#id 	#firstname 	Selects the element with id="firstname"
.class 	.intro 	Selects all elements with class="intro"
element.class 	p.intro 	Selects only <p> elements with class="intro"
* 	* 	Selects all elements
element 	p 	Selects all <p> elements
element,element,.. 	div, p 	Selects all <div> elements and all <p> elements
```



<kbd>return</kbd>[Back to table of contents](#homepage)


----------

## Link Bookmarks
HTML Links - Create Bookmarks: can enable users to jump to certain part of a webpage. This helps for a long webpage. 

* To create bookmark, create bookmark then add link to it. Clicking the page automatically redirects to boookmarked location in the webpage

-Use id attribute to create a bookmark: 
```
<h2 id="C4">Chapter 4</h2>
```
-Add link to the bookmark from within the same page.
```
 <a href="#C4">Jump to Chapter 4</a> 
```
-Add link to a bookmark on another page: 
```
<a href="html_demo.html#C4">Jump to Chapter 4</a>
```
**To remove the underline from link, remove text decoration: 
```
<a href="html_images.asp" style="text-decoration:none">HTML Images</a> 
```
Chapter Summary:

Chapter Summary

Use the id attribute (```id="value"```) to define bookmarks in a page
Use the href attribute (```href="#value"```) to link to the bookmark

<kbd>return</kbd>[Back to table of contents](#homepage)



