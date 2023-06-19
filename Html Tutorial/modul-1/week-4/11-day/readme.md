## CSS Units



CSS has several different units for expressing a length.

Many CSS properties take "length" values, such as width, margin, padding, font-size, etc.

Length is a number followed by a length unit, such as 10px, 2em, etc.

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  font-size: 60px;
}

p {
  font-size: 25px;
  line-height: 50px;
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






Note: A whitespace cannot appear between the number and the unit. However, if the value is 0, the unit can 

be omitted.

For some CSS properties, negative lengths are allowed.

There are two types of length units: absolute and relative.



Absolute Lengths

The absolute length units are fixed and a length expressed in any of these will appear as exactly that size.

Absolute length units are not recommended for use on screen, because screen sizes vary so much. However, 

they can be used if the output medium is known, such as for print layout.



Unit 	Description
cm 	centimeters
mm 	millimeters
in 	inches (1in = 96px = 2.54cm)
px * 	pixels (1px = 1/96th of 1in)
pt 	points (1pt = 1/72 of 1in)
pc 	picas (1pc = 12 pt) 


Pixels (px) are relative to the viewing device. For low-dpi devices, 1px is one device pixel (dot) of the 

display. For printers and high resolution screens 1px implies multiple device pixels.


Relative Lengths

Relative length units specify a length relative to another length property. Relative length units scales 

better between different rendering mediums.
Unit 	Description 	
em 	Relative to the font-size of the element (2em means 2 times the size of the current font) 	
ex 	Relative to the x-height of the current font (rarely used) 	
ch 	Relative to width of the "0" (zero) 	
rem 	Relative to font-size of the root element 	
vw 	Relative to 1% of the width of the viewport* 	
vh 	Relative to 1% of the height of the viewport* 	
vmin 	Relative to 1% of viewport's* smaller dimension 	
vmax 	Relative to 1% of viewport's* larger dimension 	
% 	Relative to the parent element


Tip: The em and rem units are practical in creating perfectly scalable layout!
* Viewport = the browser window size. If the viewport is 50cm wide, 1vw = 0.5cm.


NB: Always confirm browser support for the units you choose. 




What is Specificity?

If there are two or more conflicting CSS rules that point to the same element, the browser follows some 

rules to determine which one is most specific and therefore wins out.

Think of specificity as a score/rank that determines which style declarations are ultimately applied to an 

element.

The universal selector (*) has low specificity, while ID selectors are highly specific! 

Note: Specificity is a common reason why your CSS-rules don't apply to some elements, although you think 

they should.



Specificity Hierarchy

Each and every selector has its place in the hierarchy. There four categories which define the specificity 

level of a selector:


Inline styles - An inline style is attached directly to the element to be styled. Example: <h1 style="color: 

#ffffff;">.

IDs - An ID is a unique identifier for the page elements, such as #navbar.

Classes, attributes and pseudo-classes - This category includes .classes, [attributes] and pseudo-classes 

such as :hover, :focus etc.

Elements and pseudo-elements - This category includes element names and pseudo-elements, such as h1, div, 

:before and :after.


You need to memorize how to calculate specificity! This gives you better control over the elements. 

Start at 0, add 1000 for style attribute, add 100 for each ID, add 10 for each attribute, class or pseudo-

class, add 1 for each element name or pseudo-element.

Consider these three code fragments:


Example
A: h1
B: #content h1
C: <div id="content"><h1 style="color: #ffffff">Heading</h1></div>

The specificity of A is 1 (one element)
The specificity of B is 101 (one ID reference and one element)
The specificity of C is 1000 (inline styling)

Since 1 < 101 < 1000, the third rule (C) has a greater level of specificity, and therefore will be applied.



Specificity Rules

Equal specificity: the latest rule counts - If the same rule is written twice into the external style sheet, 

then the lower rule in the style sheet is closer to the element to be styled, and therefore will be applied:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {background-color: yellow;}
h1 {background-color: red;}
</style>
</head>
<body>

<h1>This is heading 1</h1>

</body>
</html>


the latter rule is always applied.

ID selectors have a higher specificity than attribute selectors - Look at the following three code lines:


<!DOCTYPE html>
<html>
<head>
<style>
div#a {background-color: green;}
#a {background-color: yellow;}
div[id=a] {background-color: blue;}
</style>
</head>
<body>

<div id="a">This is a div</div>

</body>
</html>


the first rule is more specific than the other two, and will be applied.

Contextual selectors are more specific than a single element selector - The embedded style sheet is closer 

to the element to be styled (than the external style sheet. So in the following situation, the latter rule 

will be applied.


Example
From external CSS file:
#content h1 {background-color: red;}

In HTML file:
<style>
#content h1 {
  background-color: yellow;
}
</style>



A class selector beats any number of element selectors - a class selector such as .intro beats h1, p, div, 

etc:


<!DOCTYPE html>
<html>
<head>
<style>
.intro {background-color: yellow;}
h1 {background-color: red;}
</style>
</head>
<body>

<h1 class="intro">This is a heading</h1>

</body>
</html>


The universal selector and inherited values have a specificity of 0 - *, body * and similar have a zero 

specificity. Inherited values also have a specificity of 0.


<kbd>return</kbd>[Back to table of contents](#homepage)


------


## CSS Math Functions

The CSS math functions allow mathematical expressions to be used as property values. Here, we will explain 

the calc(), max() and min() functions.


The calc() Function

The calc() function performs a calculation to be used as the property value.

CSS Syntax
calc(expression)
Value 	Description
expression 	Required. A mathematical expression. The result will be used as the value.
The following operators can be used: + - * /

See illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
#div1 {
  position: absolute;
  left: 50px;
  width: calc(100% - 100px);
  border: 1px solid black;
  background-color: yellow;
  padding: 5px;
}
</style>
</head>
<body>

<h1>The calc() Function</h1>

<p>Create a div that stretches across the window, with a 50px gap between both sides of the div and the 

edges of the window:</p>

<div id="div1">Some text...</div>

</body>
</html>


The max() Function

The max() function uses the largest value, from a comma-separated list of values, as the property value.

CSS Syntax
max(value1, value2, ...)


Value 	Description
value1, value2, ... 	Required. A list of comma-separated values - where the largest value is chosen


<!DOCTYPE html>
<html>
<head>
<style>
#div1 {
  background-color: yellow;
  height: 100px;
  width: max(50%, 300px);
}
</style>
</head>
<body>

<h1>The max() Function</h1>

<p>Use max() to set the width of #div1 to whichever value is largest, 50% or 300px:</p>

<div id="div1">Some text...</div>

<p>Resize the browser window to see the effect.</p>

</body>
</html>


The min() Function

The min() function uses the smallest value, from a comma-separated list of values, as the property value.

CSS Syntax
min(value1, value2, ...)

Value 	Description
value1, value2, ... 	Required. A list of comma-separated values - where the smallest value is chosen

Let us look at an example:


<!DOCTYPE html>
<html>
<head>
<style>
#div1 {
  background-color: yellow;
  height: 100px;
  width: min(50%, 300px);
}
</style>
</head>
<body>

<h1>The min() Function</h1>

<p>Use min() to set the width of #div1 to whichever value is smallest, 50% or 300px:</p>

<div id="div1">Some text...</div>

<p>Resize the browser window to see the effect.</p>

</body>
</html>

