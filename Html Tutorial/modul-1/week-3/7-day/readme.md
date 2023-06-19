## HTML LAYOUT
HTML LAYOUT--Layout Elements and Techniques

HTML has semantic elements 
```
<header> - Defines a header for a document or a section
<nav> - Defines a set of navigation links
<section> - Defines a section in a document
<article> - Defines an independent, self-contained content
<aside> - Defines content aside from the content (like a sidebar)
<footer> - Defines a footer for a document or a section
<etails> - Defines additional details that the user can open and close on demand
<summary> - Defines a heading for the <details> element
```

Techniques for creating HTML layouts
CSS framework
CSS float property
CSS flexbox
CSS grid

* CSS Frameworks: Enable you to fastly create your layout: W3.CSS and Boostrap are examples

CSS Float layout: Use CSS float property to do web layout. You just need to remember float and clear properties to use this. Its main disadvantage is the it is tied to the document flow which may harm flexibility.

CSS Flexbox layout::Ensures that elements behave predictably when  multiple sizes of user screen must display site well. 


CSS Gridlayout: Offers grid-based layout system which facilitate designing webpages without floats and positioning and using rows and columns to achieve this.

<kbd>return</kbd>[Back to table of contents](#homepage)


------

## HTML RESPONSIVE

HTML RESPONSIVE--Responsive Web Design;

Responsive web looks good irrespecive of the device and it automatically adjust for different sizes and viewports.

Here, HTML and CSS automatically resize, hide, shrink, or enlarge a site to make it look good on all devices (desktops, tablets, and phones)

To create a responsive site, add the following <meta> tag to all your web pages:
```

 <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
```
* Responsive Images: Scale nicely to fit any browser size. To make image responsive set CSS width property to 100 % and image will become responsive according to the needs. 
See code below for a responsive image. 
```
 <img src="img_girl.jpg" style="width:100%;"> 
```
To avoid image scaling up beyond original size, use max-width property instead of the width:100%. For exaMple:
```
 <img src="img_girl.jpg" style="max-width:100%;height:auto;"> 
```

** To show different images depending on browser width, use <picture> element.

```
<picture>
  <source srcset="img_smallflower.jpg" media="(max-width: 600px)">
  <source srcset="img_flowers.jpg" media="(max-width: 1500px)">
  <source srcset="flowers.jpg">
  <img src="img_smallflower.jpg" alt="Flowers">
</picture> 
```

** Responsive Text Size.

The text size can be set with ```"vw"``` unit, which means the ```"viewport width"```  to enable text size to follow the size ofthe browser window

* the code below enables responsive text size
```
<h1 style="font-size:10vw">Hello World</h1> 
```
* Viewport is the browser window size. 1vw = 1% of viewport width. If the viewport is 50cm wide, 1vw is 0.5cm.


* Media queries: Enables you to define completely different styles for different browser sizes. 

```
<style>
.left, .right {
  float: left;
  width: 20%; /* The width is 20%, by default */
}

.main {
  float: left;
  width: 60%; /* The width is 60%, by default */
}

/* Use a media query to add a breakpoint at 800px: */
@media screen and (max-width: 800px) {
  .left, .main, .right {
    width: 100%; /* The width is 100%, when the viewport is 800px or smaller */
  }
}
</style> 
```

* W3.CSS

W3.CSS is a modern CSS framework with support for desktop, tablet, and mobile design by default.

W3.CSS is smaller and faster than similar CSS frameworks.

W3.CSS is designed to be a high quality alternative to Bootstrap.

W3.CSS is designed to be independent of jQuery or any other JavaScript library.


** Example of a full responsive web
```
<!DOCTYPE html>
<html>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<body>

<div class="w3-container w3-green">
  <h1>W3Schools Demo</h1>
  <p>Resize this responsive page!</p>
</div>

<div class="w3-row-padding">
  <div class="w3-third">
    <h2>London</h2>
    <p>London is the capital city of England.</p>
    <p>It is the most populous city in the United Kingdom,
    with a metropolitan area of over 13 million inhabitants.</p>
  </div>

  <div class="w3-third">
    <h2>Paris</h2>
    <p>Paris is the capital of France.</p>
    <p>The Paris area is one of the largest population centers in Europe,
    with more than 12 million inhabitants.</p>
  </div>

  <div class="w3-third">
    <h2>Tokyo</h2>
    <p>Tokyo is the capital of Japan.</p>
    <p>It is the center of the Greater Tokyo Area,
    and the most populous metropolitan area in the world.</p>
  </div>
</div>

</body>
</html> 
```


** Bootstrap: another framework that uses HTML, CSS, and JQuery to make web pages:
```
<!DOCTYPE html>
<html lang="en">
<head>
<title>Bootstrap Example</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
</head>
<body>

<div class="container">
  <div class="jumbotron">
    <h1>My First Bootstrap Page</h1>
  </div>
  <div class="row">
    <div class="col-sm-4">
      ...
    </div>
    <div class="col-sm-4">
      ...
    </div>
    <div class="col-sm-4">
    ...
    </div>
  </div>
</div>

</body>
</html> 
```
<kbd>return</kbd>[Back to table of contents](#homepage)


------


## HTML SEMANTICS

HTML semantic Elements

Semantic elements are the elements that have a meaning and this meaning describes the content to both browser and the developer. 

Non-semantic element: ```<div>``` and ```<span>```   tells nothing about the content

Semantic elements: ```<form>, <table>, and <article>```  defines content
Sites usually define elements:```<div id="nav"> <div class="header"> <div id="footer">``` to indicate navigation, header, and footer.

* emantic Elements in HTML
```
<article>
<aside>
<details>
<figcaption>
<figure>
<footer>
<header>
<main>
<mark>
<nav>
<section>
<summary>
<time>
```

HTML ```<section>``` Element:  A Thematic grouping of content typically with a heading. You can split a webpage into sections for introduction, content, and contact information.
```
<section>
<h1>WWF</h1>
<p>The World Wide Fund for Nature (WWF) is an international organization working on issues regarding the conservation, research and restoration of the environment, formerly named the World Wildlife Fund. WWF was founded in 1961.</p>
</section>

<section>
<h1>WWF's Panda symbol</h1>
<p>The Panda has become the symbol of WWF. The well-known panda logo of WWF originated from a panda named Chi Chi that was transferred from the Beijing Zoo to the London Zoo in the same year of the establishment of WWF.</p>
</section> 
```


HTML ```<article>``` Element

The ```<article>``` element specifies independent self-contained content. Article should make sense and should be distributable independently from the rest of the site. Article element can be used in: Forum post, Blog post, Newspaper Article.

* Example of the usage of article elements
```
<article>
<h2>Google Chrome</h2>
<p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
</article>

<article>
<h2>Mozilla Firefox</h2>
<p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
</article>

<article>
<h2>Microsoft Edge</h2>
<p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
</article> 
```

* Use of CSS to style Article elements:
```
<html>
<head>
<style>
.all-browsers {
  margin: 0;
  padding: 5px;
  background-color: lightgray;
}

.all-browsers > h1, .browser {
  margin: 10px;
  padding: 5px;
}

.browser {
  background: white;
}

.browser > h2, p {
  margin: 4px;
  font-size: 90%;
}
</style>
</head>
<body>

<article class="all-browsers">
  <h1>Most Popular Browsers</h1>
  <article class="browser">
    <h2>Google Chrome</h2>
    <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
  </article>
  <article class="browser">
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
  </article>
  <article class="browser">
    <h2>Microsoft Edge</h2>
    <p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
  </article>
</article>

</body>
</html> 
```

Nesting ```<article>``` in ```<section>``` or Vice Versa.

The ```<article>``` element specifies independent self-contained content while <section> eleemnt defines a section in a document.

You will find HTML pages with ```<section>``` elements containing ```<article>``` element and ```<article>``` elements containing  

```
<section>
```

HTML ```<header>``` Element

```<header>```element rep a containere for introductory content or a set of navigational links and typically contains one or more ```<h1> -<h6>```, logo or icon, authorship information etc.

* Note: You can have several ```<header>``` elements in one HTML document. However, ```<header>``` cannot be placed within a ```<footer>```, ```<address>``` or another ```<header>``` element.

Example of header: 
```
<article>
  <header>
    <h1>What Does WWF Do?</h1>
    <p>WWF's mission:</p>
  </header>
  <p>WWF's mission is to stop the degradation of our planet's natural environment,
  and build a future in which humans live in harmony with nature.</p>
</article> 
```


* HTML ```<footer>``` Element

This element typically contains 
authorship information
copyright information
contact information
sitemap
back to top links
related documents
* One document can have several ```<footer>``` elements in one document


* Examples of footer section in a document
```
<footer>
  <p>Author: Hege Refsnes</p>
  <p><a href="mailto:hege@example.com">hege@example.com</a></p>
</footer> 
```

HTML ```<nav>``` Element:Defines a set of navigation links.

```<nav>``` element define a set of navigation links which are the major  blocks of navigation links. So you should not use <nav>for all links.

Browsers, such as screen readers for disabled users, can use this element to determine whether to omit the initial rendering of this content.

** A set of navigation links
```
<nav> 
  <a href="/html/">HTML</a> |
  <a href="/css/">CSS</a> |
  <a href="/js/">JavaScript</a> |
  <a href="/jquery/">jQuery</a>
</nav> 
```


HTML ```<aside>``` Element
Defines some contents aside from the content it is placed in like sidebar. The <aside> contentshould be indirectly related to the surrounding content.

```
<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

<aside>
<h4>Epcot Center</h4>
<p>Epcot is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
</aside>
```

* Using CSS to style the aside element.
```
<html>
<head>
<style>
aside {
  width: 30%;
  padding-left: 15px;
  margin-left: 15px;
  float: right;
  font-style: italic;
  background-color: lightgray;
}
</style>
</head>
<body>

<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

<aside>
<p>The Epcot center is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
</aside>

<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>
<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

</body>
</html>

```

HTML ```<figure>``` and ```<figcaption>``` Elements

The ```<figure>``` tag specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.

The ```<figcaption>``` tag defines a caption for a ```<figure>``` element. The ```<figcaption>``` element can be placed as the first or as the last child of a ```<figure>``` element.

The ```<img>``` element defines the actual image/illustration. 

* Sample code for figure and figure caption
```
<figure>
  <img src="pic_trulli.jpg" alt="Trulli">
  <figcaption>Fig1. - Trulli, Puglia, Italy.</figcaption>
</figure> 
```

* Essence of Semantic Elements
According to the W3C: "A semantic Web allows data to be shared and reused across applications, enterprises, and communities."


Semantic Elements in HTML

Below is a list of some of the semantic elements in HTML.
```
Tag 	Description
<article> 	Defines independent, self-contained content
<aside> 	Defines content aside from the page content
<details> 	Defines additional details that the user can view or hide
<figcaption> 	Defines a caption for a <figure> element
<figure> 	Specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.
<footer> 	Defines a footer for a document or section
<header> 	Specifies a header for a document or section
<main> 	Specifies the main content of a document
<mark> 	Defines marked/highlighted text
<nav> 	Defines navigation links
<section> 	Defines a section in a document
<summary> 	Defines a visible heading for a <details> element
<time> 	Defines a date/time
```
<kbd>return</kbd>[Back to table of contents](#homepage)


--------

## HTML EMOJIS

* Using Emojis in HTML

Emojis are characters from UTF-8 character set:

They look like images, or icons, but they are not. and they are letters( characters) from UTF-8 (Unicode) character set. 

UTF-8 covers almost all existing characters and symbols

<kbd>return</kbd>[Back to table of contents](#homepage)


------


## CSS Links


There are multiple ways of styling links using CSS and with the aid of CSS color, font-family, and 

background properties. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
a {
  color: hotpink;
}
</style>
</head>
<body>

<h2>CSS Links</h2>
<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>

</body>
</html>



In addition, links can be styled differently depending on what state they are in.

The four links states are:

    a:link - a normal, unvisited link
    a:visited - a link the user has visited
    a:hover - a link when the user mouses over it
    a:active - a link the moment it is clicked


When setting the style for several link states, there are some order rules:

    a:hover MUST come after a:link and a:visited
    a:active MUST come after a:hover



<!DOCTYPE html>
<html>
<head>
<style>
/* unvisited link */
a:link {
  color: red;
}

/* visited link */
a:visited {
  color: green;
}

/* mouse over link */
a:hover {
  color: hotpink;
}

/* selected link */
a:active {
  color: blue;
}
</style>
</head>
<body>

<h2>CSS Links</h2>
<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>
<p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be 

effective.</p>
<p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>

</body>
</html>



Text Decoration:::
This is mostly used to remove underlines from links. See example below:

<!DOCTYPE html>
<html>
<head>
<style>
a:link {
  text-decoration: none;
}

a:visited {
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

a:active {
  text-decoration: underline;
}
</style>
</head>
<body>

<h2>CSS Links</h2>
<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>
<p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be 

effective.</p>
<p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>

</body>
</html>




Background Color:::

The background-color property can be used to specify a background color for links:

<!DOCTYPE html>
<html>
<head>
<style>
a:link {
  background-color: yellow;
}

a:visited {
  background-color: cyan;
}

a:hover {
  background-color: lightgreen;
}

a:active {
  background-color: hotpink;
} 
</style>
</head>
<body>

<h2>CSS Links</h2>
<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>
<p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be 

effective.</p>
<p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>

</body>
</html>



Link Buttons:::

The examples below are more advanced as they combine different CSS properties to display links as  boxes/ 

buttons. See  example below:


<!DOCTYPE html>
<html>
<head>
<style>
a:link, a:visited {
  background-color: #f44336;
  color: white;
  padding: 14px 25px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: red;
}
</style>
</head>
<body>

<h2>Link Button</h2>
<p>A link styled as a button:</p>
<a href="default.asp" target="_blank">This is a link</a>

</body>
</html>


Other examples of styling CSS links

<!DOCTYPE html>
<html>
<head>
<style>
a.one:link {color:#ff0000;}
a.one:visited {color:#0000ff;}
a.one:hover {color:#ffcc00;}

a.two:link {color:#ff0000;}
a.two:visited {color:#0000ff;}
a.two:hover {font-size:150%;}

a.three:link {color:#ff0000;}
a.three:visited {color:#0000ff;}
a.three:hover {background:#66ff66;}

a.four:link {color:#ff0000;}
a.four:visited {color:#0000ff;}
a.four:hover {font-family:monospace;}

a.five:link {color:#ff0000;text-decoration:none;}
a.five:visited {color:#0000ff;text-decoration:none;}
a.five:hover {text-decoration:underline;}
</style>
</head>
<body>

<p>Mouse over the links and watch them change layout:</p>

<p><b><a class="one" href="default.asp" target="_blank">This link changes color</a></b></p>
<p><b><a class="two" href="default.asp" target="_blank">This link changes font-size</a></b></p>
<p><b><a class="three" href="default.asp" target="_blank">This link changes background-color</a></b></p>
<p><b><a class="four" href="default.asp" target="_blank">This link changes font-family</a></b></p>
<p><b><a class="five" href="default.asp" target="_blank">This link changes text-decoration</a></b></p>

</body>
</html>


Another example

<!DOCTYPE html>
<html>
<head>
<style>
a:link, a:visited {
  background-color: white;
  color: black;
  border: 2px solid green;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: green;
  color: white;
}
</style>
</head>
<body>

<a href="default.asp" target="_blank">This is a link</a>

</body>
</html>





Different types of cursors that can be used for links

<!DOCTYPE html>
<html>
<body>

<p>Mouse over the words to change the cursor.</p>
<span style="cursor:auto">auto</span><br>
<span style="cursor:crosshair">crosshair</span><br>
<span style="cursor:default">default</span><br>
<span style="cursor:e-resize">e-resize</span><br>
<span style="cursor:help">help</span><br>
<span style="cursor:move">move</span><br>
<span style="cursor:n-resize">n-resize</span><br>
<span style="cursor:ne-resize">ne-resize</span><br>
<span style="cursor:nw-resize">nw-resize</span><br>
<span style="cursor:pointer">pointer</span><br>
<span style="cursor:progress">progress</span><br>
<span style="cursor:s-resize">s-resize</span><br>
<span style="cursor:se-resize">se-resize</span><br>
<span style="cursor:sw-resize">sw-resize</span><br>
<span style="cursor:text">text</span><br>
<span style="cursor:w-resize">w-resize</span><br>
<span style="cursor:wait">wait</span><br>

</body>
</html>

<kbd>return</kbd>[Back to table of contents](#homepage)


---------


## CSS Lists

HTML Lists and CSS List properties


The unordered lists (<ul>) and ordered (<ol>) lists are the two main types of lists in HTML. Unordered lists 

are marked with bullets while ordered lists are marked with numbers or letters.


The CSS list properties allow you to:

    Set different list item markers for ordered lists
    Set different list item markers for unordered lists
    Set an image as the list item marker
    Add background colors to lists and list items



Different List Item Markers

The list-style-type property is used to specify the type of list item marker used. For example,

<!DOCTYPE html>
<html>
<head>
<style>
ul.a {
  list-style-type: circle;
}

ul.b {
  list-style-type: square;
}

ol.c {
  list-style-type: upper-roman;
}

ol.d {
  list-style-type: lower-alpha;
}
</style>
</head>
<body>

<h2>Lists</h2>
<p>Example of unordered lists:</p>
<ul class="a">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<ul class="b">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<p>Example of ordered lists:</p>
<ol class="c">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="d">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

</body>
</html>


Note: Some of the values are for unordered lists, and some for ordered lists.



An Image as the List Item Marker

The list-style-image property is used to spedify image as an item list marker. For instance,


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-image: url('sqpurple.gif');
}
</style>
</head>
<body>

<h2>CSS Lists</h2>
<p>The list-style-image property specifies an image as the list item marker:</p>

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



Position the List Item Markers

The position of the list-item markers (bullet points) is specified using list-style-position. 


"list-style-position: outside;" means that the bullet points will be outside the list item. The start of 

each line of a list item will be aligned vertically. This is default:


"list-style-position: inside;" means that the bullet points will be inside the list item. As it is part of 

the list item, it will be part of the text and push the text at the start:



<!DOCTYPE html>
<html>
<head>
<style>
ul.a {
  list-style-position: outside;
}

ul.b {
  list-style-position: inside;
}
</style>
</head>
<body>

<h1>The list-style-position Property</h1>

<h2>list-style-position: outside (default):</h2>
<ul class="a">
  <li>Coffee - A brewed drink prepared from roasted coffee beans, which are the seeds of berries from the 

Coffea plant</li>
  <li>Tea - An aromatic beverage commonly prepared by pouring hot or boiling water over cured leaves of the 

Camellia sinensis, an evergreen shrub (bush) native to Asia</li>
  <li>Coca Cola - A carbonated soft drink produced by The Coca-Cola Company. The drink's name refers to two 

of its original ingredients, which were kola nuts (a source of caffeine) and coca leaves</li>
</ul>

<h2>list-style-position: inside:</h2>
<ul class="b">
  <li>Coffee - A brewed drink prepared from roasted coffee beans, which are the seeds of berries from the 

Coffea plant</li>
  <li>Tea - An aromatic beverage commonly prepared by pouring hot or boiling water over cured leaves of the 

Camellia sinensis, an evergreen shrub (bush) native to Asia</li>
  <li>Coca Cola - A carbonated soft drink produced by The Coca-Cola Company. The drink's name refers to two 

of its original ingredients, which were kola nuts (a source of caffeine) and coca leaves</li>
</ul>

</body>
</html>




NB: Align outside is the default for list-style position and in this case, the first letter in the second 

line of each bullet content is directly under the first letter in the first line. However, when the list-

style-position is set to inside, the First letter of the second line in a list item is directly under the 

bullet symbol in the first line.   



Remove Default Settings

The list-style-type:none property can also be used to remove the markers/bullets. Note that the list also 

has default margin and padding. To remove this, add margin:0 and padding:0 to <ul> or <ol>:

<!DOCTYPE html>
<html>
<head>
<style>
ul.demo {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
</style>
</head>
<body>

<p>Default list:</p>
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<p>Remove bullets, margin and padding:</p>
<ul class="demo">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



List - Shorthand property

The list-style property is a shorthand property. It is used to set all the list properties in one 

declaration:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style: square inside url("sqpurple.gif");
}
</style>
</head>
<body>

<h2>CSS Lists</h2>
<p>The list-style property is a shorthand property, which is used to set all the list properties in one 

declaration.</p>

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



When using the shorthand property, the order of the property values are:

1. list-style-type (if a list-style-image is specified, the value of this property will be displayed if the 

image for some reason cannot be displayed)
2. list-style-position (specifies whether the list-item markers should appear inside or outside the content 

flow)
3. list-style-image (specifies an image as the list item marker)

If one of the property values above are missing, the default value for the missing property will be 

inserted, if any.


Styling List With Colors

We can also style lists with colors, to make them look a little more interesting.

Anything added to the <ol> or <ul> tag, affects the entire list, while properties added to the <li> tag will 

affect the individual list items:



<!DOCTYPE html>
<html>
<head>
<style>
ol {
  background: #ff9999;
  padding: 20px;
}

ul {
  background: #3399ff;
  padding: 20px;
}

ol li {
  background: #ffe5e5;
  padding: 5px;
  margin-left: 35px;
}

ul li {
  background: #cce5ff;
  margin: 5px;
}
</style>
</head>
<body>

<h1>Styling Lists With Colors:</h1>

<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



More examples:

Customized list with a red left border:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  border-left: 5px solid red;
  background-color: #f1f1f1;
  list-style-type: none;
  padding: 10px 20px;
}
</style>
</head>
<body>

<p>List with a red left border:</p>
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>


Full width bordered list:

<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  padding: 0;
  border: 1px solid #ddd;
}

ul li {
  padding: 8px 16px;
  border-bottom: 1px solid #ddd;
}

ul li:last-child {
  border-bottom: none
}
</style>
</head>
<body>

<p>Full-width bordered list:</p>
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



All the different list-item markers for lists:


<!DOCTYPE html>
<html>
<head>
<style>
ul.a {list-style-type: circle;}
ul.b {list-style-type: disc;}
ul.c {list-style-type: square;}

ol.d {list-style-type: armenian;}
ol.e {list-style-type: cjk-ideographic;}
ol.f {list-style-type: decimal;}
ol.g {list-style-type: decimal-leading-zero;}
ol.h {list-style-type: georgian;}
ol.i {list-style-type: hebrew;}
ol.j {list-style-type: hiragana;}
ol.k {list-style-type: hiragana-iroha;}
ol.l {list-style-type: katakana;}
ol.m {list-style-type: katakana-iroha;}
ol.n {list-style-type: lower-alpha;}
ol.o {list-style-type: lower-greek;}
ol.p {list-style-type: lower-latin;}
ol.q {list-style-type: lower-roman;}
ol.r {list-style-type: upper-alpha;}
ol.s {list-style-type: upper-latin;}
ol.t {list-style-type: upper-roman;}
ol.u {list-style-type: none;}
ol.v {list-style-type: inherit;}
</style>
</head>
<body>

<ul class="a">
  <li>Circle type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<ul class="b">
  <li>Disc type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<ul class="c">
  <li>Square type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<ol class="d">
  <li>Armenian type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="e">
  <li>Cjk-ideographic type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="f">
  <li>Decimal type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="g">
  <li>Decimal-leading-zero type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="h">
  <li>Georgian type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="i">
  <li>Hebrew type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="j">
  <li>Hiragana type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="k">
  <li>Hiragana-iroha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="l">
  <li>Katakana type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="m">
  <li>Katakana-iroha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="n">
  <li>Lower-alpha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="o">
  <li>Lower-greek type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="p">
  <li>Lower-latin type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="q">
  <li>Lower-roman type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="r">
  <li>Upper-alpha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="s">
  <li>Upper-latin type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="t">
  <li>Upper-roman type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="u">
  <li>None type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="v">
  <li>inherit type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

</body>
</html>

<kbd>return</kbd>[Back to table of contents](#homepage)


-------



## CSS Tables

CSS helps to improve the appearance of HTML tables


An example of table is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
#customers {
  font-family: Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

#customers td, #customers th {
  border: 1px solid #ddd;
  padding: 8px;
}

#customers tr:nth-child(even){background-color: #f2f2f2;}

#customers tr:hover {background-color: #ddd;}

#customers th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #04AA6D;
  color: white;
}
</style>
</head>
<body>

<table id="customers">
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Berglunds snabbköp</td>
    <td>Christina Berglund</td>
    <td>Sweden</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
  <tr>
    <td>Ernst Handel</td>
    <td>Roland Mendel</td>
    <td>Austria</td>
  </tr>
  <tr>
    <td>Island Trading</td>
    <td>Helen Bennett</td>
    <td>UK</td>
  </tr>
  <tr>
    <td>Königlich Essen</td>
    <td>Philip Cramer</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Laughing Bacchus Winecellars</td>
    <td>Yoshi Tannamuri</td>
    <td>Canada</td>
  </tr>
  <tr>
    <td>Magazzini Alimentari Riuniti</td>
    <td>Giovanni Rovelli</td>
    <td>Italy</td>
  </tr>
  <tr>
    <td>North/South</td>
    <td>Simon Crowther</td>
    <td>UK</td>
  </tr>
  <tr>
    <td>Paris spécialités</td>
    <td>Marie Bertrand</td>
    <td>France</td>
  </tr>
</table>

</body>
</html>




Table Borders


Table Borders

To specify table borders in CSS, use the border property.

The example below specifies a black border for <table>, <th>, and <td> elements:


<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
}
</style>
</head>
<body>

<h2>Add a border to a table:</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
  </tr>
</table>

</body>
</html>



Full-Width Table:


If you wish to create a table that will span the entire screen (full-width), add width:100% to the <table>
 elemnt as shown below:



<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
}

table {
  width: 100%;
}
</style>
</head>
<body>

<h2>Full-width Table</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
  </tr>
</table>

</body>
</html>




Double Borders

Notice that the table in the examples above have double borders. This is because both the table and the <th> 

and <td> elements have separate borders.

To remove double borders, take a look at the example below.




<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  width: 100%;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Let the borders collapse</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
  </tr>
</table>

</body>
</html>



To create a table with just border around the table, only specify border property for <table> 


<!DOCTYPE html>
<html>
<head>
<style>
table {
  width: 100%;
  border-collapse: collapse;
  border: 1px solid black;
}
</style>
</head>
<body>

<h2>Single Border Around The Table</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
  </tr>
</table>

</body>
</html>



Table Size

Table Width and Height

The width and height of a table are defined by the width and height properties.

The example below sets the width of the table to 100%, and the height of the <th> elements to 70px:



<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 100%;
}

th {
  height: 70px;
}
</style>
</head>
<body>

<h2>The width and height Properties</h2>
<p>Set the width of the table, and the height of the table header row:</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



To create a table that should only span half of the page, use the width:50% specification.  See illustration 

below:


<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 50%;
}

th {
  height: 70px;
}
</style>
</head>
<body>

<h2>The width and height Properties</h2>
<p>Set the width of the table, and the height of the table header row:</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>


CSS Table Alignment::

Horizontal Alignment

The text-align property sets the horizontal alignment (like left, right, or center) of the content in <th> 

or <td>.

By default, the content of <th> elements are center-aligned and the content of <td> elements are left-

aligned.

To center-align the content of  <td> elements as well, use text-align: center:



<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 100%;
}

td {
  text-align: center;
}
</style>
</head>
<body>

<h2>The text-align Property</h2>
<p>This property sets the horizontal alignment (like left, right, or center) of the content in th or td.</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



To left-align the content, force the alignment of <th> elements to be left-aligned, with the text-align: 

left property:


<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 100%;
}

th {
  text-align: left;
}
</style>
</head>
<body>

<h2>The text-align Property</h2>
<p>This property sets the horizontal alignment (like left, right, or center) of the content in th or td.</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



Vertical Alignment


The vertical-align property sets the vertical alignment (like top, bottom, or middle) of the content in <th> 

or <td>. By default, the vertical alignment of the content in a table is middle (for both <th> and <td> 

elements).

The following example sets the vertical text alignment to bottom for <td> elements:

<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 100%;
}

td {
  height: 50px;
  vertical-align: bottom;
}
</style>
</head>
<body>

<h2>The vertical-align Property</h2>
<p>This property sets the vertical alignment (like top, bottom, or middle) of the content in th or td.</p>
<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>


CSS Table Style

Table Padding

To control the space between the border and the content in a table, use the padding property on <td> and 

<th> elements:

<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {  
  border: 1px solid #ddd;
  text-align: left;
}

table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  padding: 15px;
}
</style>
</head>
<body>

<h2>The padding Property</h2>
<p>This property adds space between the border and the content in a table.</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



Horizontal Dividers

Add the border-bottom property to <th> and <td> for horizontal dividers:


<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  padding: 8px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}
</style>
</head>
<body>

<h2>Bordered Table Dividers</h2>
<p>Add the border-bottom property to th and td for horizontal dividers:</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>





Hoverable Table

Use the :hover selector on <tr> to highlight table rows on mouse over:



<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  padding: 8px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}

tr:hover {background-color: yellow;}
</style>
</head>
<body>

<h2>Hoverable Table</h2>
<p>Move the mouse over the table rows to see the effect.</p>

<table>
  <tr>
    <th>First Name</th>
    <th>Last Name</th>
    <th>Points</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



Striped Tables

For zebra-striped tables, use the nth-child() selector and add a background-color to all even (or odd) table 

rows:

first row is the heading (odd beginning with <th>)



<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {background-color: #f2f2f2;}
</style>
</head>
<body>

<h2>Striped Table</h2>
<p>For zebra-striped tables, use the nth-child() selector and add a background-color to all even (or odd) 

table rows:</p>

<table>
  <tr>
  <th>First Name</th>
  <th>Last Name</th>
  <th>Points</th>
  </tr>
  <tr>
  <td>Peter</td>
  <td>Griffin</td>
  <td>$100</td>
  </tr>
  <tr>
  <td>Lois</td>
  <td>Griffin</td>
  <td>$150</td>
  </tr>
  <tr>
  <td>Joe</td>
  <td>Swanson</td>
  <td>$300</td>
  </tr>
  <tr>
  <td>Cleveland</td>
  <td>Brown</td>
  <td>$250</td>
  </tr>
</table>

</body>
</html>




Table Color

The example below specifies the background color and text color of <th> elements:

<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  text-align: left;
  padding: 8px;
}

tr:nth-child(even){background-color: #f2f2f2}

th {
  background-color: #04AA6D;
  color: white;
}
</style>
</head>
<body>

<h2>Colored Table Header</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
</tr>
</table>

</body>
</html>




CSS Responsive Table

Responsive Table

A responsive table will display a horizontal scroll bar if the screen is too small to display the full 

content:

Add a container element (like <div>) with overflow-x:auto around the <table> element to make it responsive:


Note: In OS X Lion (on Mac), scrollbars are hidden by default and only shown when being used (even though 

"overflow:scroll" is set).

<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {background-color: #f2f2f2;}
</style>
</head>
<body>

<h2>Responsive Table</h2>
<p>A responsive table will display a horizontal scroll bar if the screen is too 
small to display the full content. Resize the browser window to see the effect:</p>
<p>To create a responsive table, add a container element (like div) with <strong>overflow-x:auto</strong> 

around the table element:</p>

<div style="overflow-x:auto;">
  <table>
    <tr>
      <th>First Name</th>
      <th>Last Name</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
    </tr>
    <tr>
      <td>Jill</td>
      <td>Smith</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
    </tr>
    <tr>
      <td>Eve</td>
      <td>Jackson</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
    </tr>
    <tr>
      <td>Adam</td>
      <td>Johnson</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
    </tr>
  </table>
</div>

</body>
</html>



More table examples:


To make a fancy table


<!DOCTYPE html>
<html>
<head>
<style>
#customers {
  font-family: Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

#customers td, #customers th {
  border: 1px solid #ddd;
  padding: 8px;
}

#customers tr:nth-child(even){background-color: #f2f2f2;}

#customers tr:hover {background-color: #ddd;}

#customers th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #04AA6D;
  color: white;
}
</style>
</head>
<body>

<table id="customers">
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Berglunds snabbköp</td>
    <td>Christina Berglund</td>
    <td>Sweden</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
  <tr>
    <td>Ernst Handel</td>
    <td>Roland Mendel</td>
    <td>Austria</td>
  </tr>
  <tr>
    <td>Island Trading</td>
    <td>Helen Bennett</td>
    <td>UK</td>
  </tr>
  <tr>
    <td>Königlich Essen</td>
    <td>Philip Cramer</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Laughing Bacchus Winecellars</td>
    <td>Yoshi Tannamuri</td>
    <td>Canada</td>
  </tr>
  <tr>
    <td>Magazzini Alimentari Riuniti</td>
    <td>Giovanni Rovelli</td>
    <td>Italy</td>
  </tr>
  <tr>
    <td>North/South</td>
    <td>Simon Crowther</td>
    <td>UK</td>
  </tr>
  <tr>
    <td>Paris spécialités</td>
    <td>Marie Bertrand</td>
    <td>France</td>
  </tr>
</table>

</body>
</html>




To set the position of table caption

<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

caption {
  caption-side: bottom;
}
</style>
</head>
<body>

<table>
<caption>Table 1.1 Customers</caption>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr class="alt">
    <td>Berglunds snabbköp</td>
    <td>Christina Berglund</td>
    <td>Sweden</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
  <tr class="alt">
    <td>Ernst Handel</td>
    <td>Roland Mendel</td>
    <td>Austria</td>
  </tr>
  <tr>
    <td>Island Trading</td>
    <td>Helen Bennett</td>
    <td>UK</td>
  </tr>
</table>

</body>
</html>

<kbd>return</kbd>[Back to table of contents](#homepage)


--------





## CSS Position

CSS Layout - The position Property

The position property is used to specify whether the positioning of an element is static, relative, fixed, 

absolute, or sticky. The elements are then positioned using top, bottom, left, and right properties (these 

properties only work after position property is first set). These properties work differently depending on 

the CSS position set.



position: static;  ::

Static position is the default for all html elements. Static positioned element are not affected by top 

bottom, left, and right properties. They are not positioned in a special way but rather follow the normal 

flow of the page. See the illustration of the usage of position;static; below. 

<!DOCTYPE html>
<html>
<head>
<style>
div.static {
  position: static;
  border: 3px solid #73AD21;
}
</style>
</head>
<body>

<h2>position: static;</h2>

<p>An element with position: static; is not positioned in any special way; it is 
always positioned according to the normal flow of the page:</p>

<div class="static">
  This div element has position: static;
</div>

</body>
</html>




position:relative;  ::

The relative position property enables an element to be positioned relative to its normal position. Settng 

the top,right, bottom, and left properties of an element with position: relative; adjusts such element from 

its normal position. The rest of the contents do not occupy any gap left by the element. See an illustration 

below:


<!DOCTYPE html>
<html>
<head>
<style>
div.relative {
  position: relative;
  left: 30px;
  border: 3px solid #73AD21;
}
</style>
</head>
<body>

<h2>position: relative;</h2>

<p>An element with position: relative; is positioned relative to its normal position:</p>

<div class="relative">
This div element has position: relative;
</div>

</body>
</html>




NB: left: 30px;  position the element 30px away from its original position (moved to the right by 30px).




position: fixed; ::

This enables an element positioning relative to the viewport; element stays in the same place even if page 

is scrolled. A fixed element does not leave a gap in the page where it would normally have been located.

The top, right, bottom, and left properties are used to position the element.


See example below:


<!DOCTYPE html>
<html>
<head>
<style>
div.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;
}
</style>
</head>
<body>

<h2>position: fixed;</h2>

<p>An element with position: fixed; is positioned relative to the viewport, which means it always stays in 

the same place even if the page is scrolled:</p>

<div class="fixed">
This div element has position: fixed;
</div>

</body>
</html>

NB: bottom:0; right:0; means that the element is positioned in the right bottom corner exactly without any 

gap between the element borders and the viewport.




position: absolute; ::

An element with position:absolute; is positioned relative to its closest ancestor, rather than position 

relative to the viewport. The absolute positioned element uses the document body as ancestor if it has no 

positioned ancestor, and they move along with page scrolling. See example below:


Note: Absolute positioned elements are removed from the normal flow, and can overlap elements.



<!DOCTYPE html>
<html>
<head>
<style>
div.relative {
  position: relative;
  width: 400px;
  height: 200px;
  border: 3px solid #73AD21;
} 

div.absolute {
  position: absolute;
  top: 80px;
  right: 0;
  width: 200px;
  height: 100px;
  border: 3px solid #73AD21;
}
</style>
</head>
<body>

<h2>position: absolute;</h2>

<p>An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of 

positioned relative to the viewport, like fixed):</p>

<div class="relative">This div element has position: relative;
  <div class="absolute">This div element has position: absolute;</div>
</div>

</body>
</html>



Position: sticky; :::

An element positioned as sticky is positioned relative the the user's position during scrolling. The stick 

element position is toggled between relative and fixed depending on the scroll position. It is positioned 

relative until a given offset position is met in the viewport - then it "sticks" in place (like 

position:fixed). You must also specify top, right, bottom, or left position for sticky position to work. 


To  make the sticky elemnt sticks to the top of the page (top: 0) when you reach its scroll position, see 

how to do it below:


<!DOCTYPE html>
<html>
<head>
<style>
div.sticky {
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  padding: 5px;
  background-color: #cae8ca;
  border: 2px solid #4CAF50;
}
</style>
</head>
<body>

<p>Try to <b>scroll</b> inside this frame to understand how sticky positioning works.</p>

<div class="sticky">I am sticky!</div>

<div style="padding-bottom:2000px">
  <p>In this example, the sticky element sticks to the top of the page (top: 0), when you reach its scroll 

position.</p>
  <p>Scroll back up to remove the stickyness.</p>
  <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
  <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
</div>

</body>
</html>



Overlapping elements::

The positioned elements can overlap other elements.  The z-index property specifies the order of stacking 

the element (which element should be placed in front of (z is positive) or behind (z is negative) the 

others). The z-index can be positive or negative.

<!DOCTYPE html>
<html>
<head>
<style>
img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<img src="w3css.gif" width="100" height="140">
<p>Because the image has a z-index of -1, it will be placed behind the text.</p>

</body>
</html>



An element with greater stack order is always in front of an element with a lower stack order.

Note: If two positioned elements overlap without a z-index specified, the element positioned last in the 

HTML code will be shown on top.



Positioning Text In an Image.


Top left:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.topleft {
  position: absolute;
  top: 8px;
  left: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Add some text to an image in the top left corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="topleft">Top Left</div>
</div>

</body>
</html>


Top right:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.topright {
  position: absolute;
  top: 8px;
  right: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Add some text to an image in the top right corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="topright">Top Right</div>
</div>

</body>
</html>




Bottom left:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.bottomleft {
  position: absolute;
  bottom: 8px;
  left: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Add some text to an image in the bottom left corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="bottomleft">Bottom Left</div>
</div>

</body>
</html>



Bottom Right:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.bottomright {
  position: absolute;
  bottom: 8px;
  right: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Add some text to an image in the bottom right corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="bottomright">Bottom Right</div>
</div>

</body>
</html>




Centered::

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.center {
  position: absolute;
  top: 50%;
  width: 100%;
  text-align: center;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Center text in image:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="center">Centered</div>
</div>

</body>
</html>



To set the shape of an element::

<!DOCTYPE html>
<html>
<head>
<style>
img {
  position: absolute;
  clip: rect(0px,60px,200px,0px);
}
</style>
</head>
<body>

<img src="w3css.gif" width="100" height="140">

</body>
</html>




All CSS Positioning Properties
Property 	Description
bottom 	Sets the bottom margin edge for a positioned box
clip 	Clips an absolutely positioned element
left 	Sets the left margin edge for a positioned box
position 	Specifies the type of positioning for an element
right 	Sets the right margin edge for a positioned box
top 	Sets the top margin edge for a positioned box
z-index 	Sets the stack order of an element


NB: position, left:-20px; means that the element is moved 20px left away from its normal position.
      
<kbd>return</kbd>[Back to table of contents](#homepage)


------




## CSS Z-index
CSS Layout - The z-index Property

The z-index Property

When elements are positioned, they can overlap other elements.

The z-index property specifies the stack order of an element (which element should be placed in front of, or behind, the others). See the illustration of CSS z-index below:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<img src="w3css.gif" width="100" height="140">
<p>Because the image has a z-index of -1, it will be placed behind the text.</p>

</body>
</html>

Note: z-index only works on positioned elements (position: absolute, position: relative, position: fixed, or position: sticky) and flex items (elements that are direct children of display: flex elements).   
      
Another z-index Example
Example

Here we see that an element with greater stack order is always above an element with a lower stack order:
<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.black-box {
  position: relative;
  z-index: 1;
  border: 2px solid black;
  height: 100px;
  margin: 30px;
}

.gray-box {
  position: absolute;
  z-index: 3; /* gray box will be above both green and black box */
  background: lightgray;
  height: 60px;  
  width: 70%;
  left: 50px;
  top: 50px;
}

.green-box {
  position: absolute;
  z-index: 2; /* green box will be above black box */
  background: lightgreen;
  width: 35%;
  left: 270px;
  top: -15px;
  height: 100px;
}
</style>
</head>
<body>

<h1>Z-index Example</h1>

<p>An element with greater stack order is always above an element with a lower stack order.</p>

<div class="container">
  <div class="black-box">Black box (z-index: 1)</div>
  <div class="gray-box">Gray box (z-index: 3)</div>
  <div class="green-box">Green box (z-index: 2)</div>
</div>

</body>
</html>

Without z-index

If two positioned elements overlap each other without a z-index specified, the element defined last in the HTML code will be shown on top.
Example

Same example as above, but here with no z-index specified:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.black-box {
  position: relative;
  border: 2px solid black;
  height: 100px;
  margin: 30px;
}

.gray-box {
  position: absolute;
  background: lightgray;
  height: 60px;  
  width: 70%;
  left: 50px;
  top: 50px;
}

.green-box {
  position: absolute;
  background: lightgreen;
  width: 35%;
  left: 270px;
  top: -15px;
  height: 100px;
}
</style>
</head>
<body>

<h1>Overlapping elements</h1>

<p>If two positioned elements overlap each other without a z-index specified,
the element defined last in the HTML code will be shown on top:</p>

<div class="container">
  <div class="black-box">Black box</div>
  <div class="gray-box">Gray box</div>
  <div class="green-box">Green box</div>
</div>

</body>
</html>

CSS Property
Property 	Description
z-index 	Sets the stack order of an element
      
      
<kbd>return</kbd>[Back to table of contents](#homepage)




## CSS Overflow
CSS Layout - Overflow

States what happens if text exceed the space provided for it to occcupy.

An illustration of this property is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
#overflowTest {
  background: #4CAF50;
  color: white;
  padding: 15px;
  width: 50%;
  height: 100px;
  overflow: scroll;
  border: 1px solid #ccc;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>The overflow property controls what happens to content that is too big to fit into an area.</p>

<div id="overflowTest">This text is really long and the height of its container is only 100 pixels. 

Therefore, a scrollbar is added to help the reader to scroll the content. Lorem ipsum dolor sit amet, 

consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat 

volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut 

aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse 

molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio 

dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber 

tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim 

assum. Typi non habent claritatem insitam; est usus legentis in iis qui facit eorum claritatem.</div>

</body>
</html>




CSS Overflow

Specifies whether the introduction of scroll bars or clipping content will occur when content of  an element 

is too big to fit in the specified area.


Properties of overflow property:
visible:This is the default, and ensures that the overflow is not clipped. Content appears outside the 

element's box. 

hidden: clips the overflow, making the remaining content of the element visible
scroll: clips the overflow, adding scrollbars with which the rest of the content of the element would be 

seen. 
auto: Works similar to scroll, just that it adds scroll bars only when necessary. 

NB: Overflow property works for block elements which has specified height. Also,

In OS X Lion (on Mac), scrollbars are hidden by default and only shown when being used (even though 

"overflow:scroll" is set).



overflow: visible;  ::

this is the default value for overflow. It is not clipped and renders outside the element's box. See the 

illustration of overflow: visible below:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 50px;
  border: 1px dotted black;
  overflow: visible;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>By default, the overflow is visible, meaning that it is not clipped and it renders outside the element's 

box:</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>


overflow: hidden; ::

The hidden overflow property value is clipped (fits inside the provided box), and the rest of the content is 

hidden. See illustration of overflow: hidden; below:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 50px;
  border: 1px dotted black;
  overflow: hidden;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>With the hidden value, the overflow is clipped, and the rest of the content is hidden:</p>
<p>Try to remove the overflow property to understand how it works.</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>



overflow: scroll; ::

When the overflow is set to scroll, such overflow is clipped and a scrollbar is added inside the box. This 

option adds both horizontal and vertical scroll bars, even in circumstances where they are not needed. See 

an illustration of overflow: scroll; below:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 100px;
  border: 1px dotted black;
  overflow: scroll;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>Setting the overflow value to scroll, the overflow is clipped and a scrollbar is added to scroll inside 

the box. Note that this will add a scrollbar both horizontally and vertically (even if you do not need 

it):</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>



overflow: auto; ::

The overflow:auto; is similar to scroll, but only add scrollbars only when it is necessary. In essence, it 

resolves issues of useless scrollbars that arise when overflow:scroll; is used. See illustration of 

overflow:auto; below:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 50px;
  border: 1px dotted black;
  overflow: auto;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>The auto value is similar to scroll, only it add scrollbars when necessary:</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>



overflow-x and overflow-y; ::

overflow-x and overflow-y property enable setting overflow of content to only horizontal, just vertical, or 

both. This can give similar advantage given by overflow: auto: over overflow:scroll;
See illustration of overflow-x and overflow-y below:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 50px;
  border: 1px dotted black;
  overflow-x: hidden;
  overflow-y: scroll;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>You can also change the overflow of content horizontally or vertically.</p>
<p>overflow-x specifies what to do with the left/right edges of the content.<br>
overflow-y specifies what to do with the top/bottom edges of the content.</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>



All CSS Overflow Properties
Property 	Description
overflow 	Specifies what happens if content overflows an element's box
overflow-x 	Specifies what to do with the left/right edges of the content if it overflows the element's 

content area
overflow-y 	Specifies what to do with the top/bottom edges of the content if it overflows the element's 

content area

<kbd>return</kbd>[Back to table of contents](#homepage)


------------


