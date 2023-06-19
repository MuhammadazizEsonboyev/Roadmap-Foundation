## HTML MEDIA
PART 5: HTML MEDIA

HTML Multimedia:

Multimedia on the web is sound, music, videos, movies, and animations.

Multimedia files have formats and different extensions like: .wav, .mp3, .mp4, .mpg, .wmv, and .avi.

* Videoformats

Format 	File 	Description
MPEG 	.mpg
.mpeg 	MPEG. Developed by the Moving Pictures Expert Group. The first popular video format on the web. Not supported anymore in HTML.


AVI 	.avi 	AVI (Audio Video Interleave). Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers.

WMV 	.wmv 	WMV (Windows Media Video). Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers.


QuickTime 	.mov 	QuickTime. Developed by Apple. Commonly used in video cameras and TV hardware. Plays well on Apple computers, but not in web browsers.


RealVideo 	.rm
.ram 	RealVideo. Developed by Real Media to allow video streaming with low bandwidths. Does not play in web browsers.


Flash 	.swf
.flv 	Flash. Developed by Macromedia. Often requires an extra component (plug-in) to play in web browsers.


Ogg 	.ogg 	Theora Ogg. Developed by the Xiph.Org Foundation. Supported by HTML.


WebM 	.webm 	WebM. Developed by Mozilla, Opera, Adobe, and Google. Supported by HTML.

MPEG-4
or MP4 	.mp4 	MP4. Developed by the Moving Pictures Expert Group. Commonly used in video cameras and TV hardware. Supported by all browsers and  recommended by YouTube.  


Note: Only MP4, WebM, and Ogg video are supported by the HTML standard.



* Common Audio formats:Only MP3, WAV, and Ogg audio are supported by the HTML standard. MP3 is the best format for compressed recorded music. The term MP3 has become synonymous with digital music. If your website is about recorded music, MP3 is the choice.


Format 	File 	Description

MIDI 	.mid
.midi 	MIDI (Musical Instrument Digital Interface). Main format for all electronic music devices like synthesizers and PC sound cards. MIDI files do not contain sound, but digital notes that can be played by electronics. Plays well on all computers and music hardware, but not in web browsers.


RealAudio 	.rm
.ram 	RealAudio. Developed by Real Media to allow streaming of audio with low bandwidths. Does not play in web browsers.


WMA 	.wma 	WMA (Windows Media Audio). Developed by Microsoft. Plays well on Windows computers, but not in web browsers.


AAC 	.aac 	AAC (Advanced Audio Coding). Developed by Apple as the default format for iTunes. Plays well on Apple computers, but not in web browsers.


WAV 	.wav 	WAV. Developed by IBM and Microsoft. Plays well on Windows, Macintosh, and Linux operating systems. Supported by HTML.


Ogg 	.ogg 	Ogg. Developed by the Xiph.Org Foundation. Supported by HTML.


MP3 	.mp3 	MP3 files are actually the sound part of MPEG files. MP3 is the most popular format for music players. Combines good compression (small files) with high quality. Supported by all browsers.

MP4 	.mp4 	MP4 is a video format, but can also be used for audio. Supported by all browsers.
<kbd>return</kbd>[Back to table of contents](#homepage)


---------


## HTML VIDEO

The ```<video>``` element is used to shows a video on a page. 

```
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

"controls" attribute adds video controls like play, pause, and volume. It is good to include width and height attributes. Without setting these, the page may move irregularly or unsteadily as the video loads. 

The ```<source>``` element allows specifying alternative video files that the browser may choose from. The browser by default chooses the first recognized format. The text between video tags will only be displayed if browser does not support the <video> element. 

* HTML ```<video>``` Autoplay

* Autoplay attribute starts video automatically. 
```
<video width="320" height="240" autoplay>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```
The autoplay attribute does not work in mobile devices like iPad and iPhone.

* HTML Video Formats

There are three supported video formats: MP4, WebM, and Ogg. The browser support for the different formats is:
Browser 	MP4 	WebM 	Ogg
Edge 	YES 	YES 	YES
Chrome 	YES 	YES 	YES
Firefox 	YES 	YES 	YES
Safari 	YES 	YES 	NO
Opera 	YES 	YES 	YES


* HTML Video - Media Types
File Format 	Media Type
MP4 	video/mp4
WebM 	video/webm
Ogg 	video/ogg

* HTML Video - Methods, Properties, and Events

The HTML DOM defines methods, properties, and events for the <video> element.

This allows you to load, play, and pause videos, as well as setting duration and volume.

There are also DOM events that can notify you when a video begins to play, is paused, etc.


* See HTML video audio DOM reference for details of how to customize video in HTML

Summary
HTML Video Tags
Tag 	Description
```
<video> 	Defines a video or movie
<source> 	Defines multiple media resources for media elements, such as <video> and <audio>
<track> 	Defines text tracks in media players
```
<kbd>return</kbd>[Back to table of contents](#homepage)

------



## HTML AUDIO

HTML ```<audio>``` element

The ```<audio>``` element is used to play an audio file. 
```
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio> 
```

* HTML Audio - How It Works

The controls attribute adds audio controls, like play, pause, and volume.

The ```<source>``` element allows you to specify alternative audio files which the browser may choose from. The browser will use the first recognized format.

The text between the ```<audio>``` and ```</audio>``` tags will only be displayed in browsers that do not support the ```<audio>``` element.


There are three supported audio format: MP3, WAV, OGG. 


Opera, Firefox and Chrome support all audio formats. Edge/Internet explorer supports only MP3 while Safari supports only MP3 and WAV.


HTML Audio - Media Types
File Format 	Media Type
MP3 	audio/mpeg
OGG 	audio/ogg
WAV 	audio/wav


* HTML Audio - Methods, Properties, and Events

The HTML DOM defines methods, properties, and events for the ```<audio>``` element.

This allows you to load, play, and pause audios, as well as set duration and volume.

There are also DOM events that can notify you when an audio begins to play, is paused, etc.

For a full DOM reference, go to w3c HTML Audio/Video DOM Reference.

HTML Audio Tags
Tag 	Description
```<audio>``` 	Defines sound content
```<source>``` 	Defines multiple media resources for media elements, such as <video> and <audio>
<kbd>return</kbd>[Back to table of contents](#homepage)


-------


## HTML YOUTUBE

HTML YouTube Videos

This is the easiest way to play videos in HTML because it removes the necessity of converting to different formats. YouTube can be allowed to play videos on your website to avoid the conversion problem. 


* YouTube Video Id

YouTube will display an id (like tgbNymZ7vqY), when you save (or play) a video.

You can use this id, and refer to your video in the HTML code.

* Playing YouTube in HTML

To play your video on a web page, do the following:
Upload the video to YouTube
Take a note of the video id
Define an <iframe> element in your web page
Let the src attribute point to the video URL
Use the width and height attributes to specify the dimension of the player
Add any other parameters to the URL (see below)

```
<iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY">
</iframe>
```

* YouTube Autoplay + Mute

You can let your video start playing automatically when a user visits the page, by adding autoplay=1 to the YouTube URL.

Note: Automatically starting a video can annoy your visitor and end up causing more harm than good!

Chrome added stricter autoplay policies in 2018. Chromium browsers do not allow autoplay in all cases. However, muted autoplay is always allowed.

Add mute=1 after autoplay=1 to let your video start playing automatically (but muted).

```
<iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY?autoplay=1&mute=1">
</iframe>
```
```
 <iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
</iframe>
```

```
<iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
</iframe>
```

* YouTube Controls

Add controls=0 to display controls in the video player.

Value 0: Player controls does not display.

Value 1 (default): Player controls display.

```
<iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY?controls=0">
</iframe>
```
<kbd>return</kbd>[Back to table of contents](#homepage)


---------


## CSS Inline-block

CSS Layout - display: inline-block;

The display: inline-block Value:

Unlike display:inline; which does not respect the top and bottom margins/ paddings, display:inline-block 

respects the top and bottom margins/ paddings and also allows one to set a width and height on the element. 

Compared to display:block; the display:inline-block does not add a line-break after the element, so the 

element can sit next to other elements.Note that display:inline; is the default for span. See the 

illustration of the difference between display: inline; , display: inline-block; , and display:block;


<!DOCTYPE html>
<html>
<head>
<style>
span.a {
  display: inline; /* the default for span */
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;  
  background-color: yellow; 
}

span.b {
  display: inline-block;
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;    
  background-color: yellow; 
}

span.c {
  display: block;
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;    
  background-color: yellow; 
}
</style>
</head>
<body>

<h1>The display Property</h1>

<h2>display: inline</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet 

consequat. Aliquam erat volutpat. <span class="a">Aliquam</span> <span class="a">venenatis</span> gravida 

nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

<h2>display: inline-block</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet 

consequat. Aliquam erat volutpat. <span class="b">Aliquam</span> <span class="b">venenatis</span> gravida 

nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

<h2>display: block</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet 

consequat. Aliquam erat volutpat. <span class="c">Aliquam</span> <span class="c">venenatis</span> gravida 

nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

</body>
</html>


Using inline-block to create navigation links;

A common application of display:inline-block is displaying list items horizontally instead of vertically. 

See below for an example of a horizontal navigation links:


<!DOCTYPE html>
<html>
<head>
<style>
.nav {
  background-color: yellow; 
  list-style-type: none;
  text-align: center;
  margin: 0;
  padding: 0;
}

.nav li {
  display: inline-block;
  font-size: 20px;
  padding: 20px;
}
</style>
</head>
<body>

<h1>Horizontal Navigation Links</h1>
<p>By default, list items are displayed vertically. In this example we use display: inline-block to display 

them horizontally (side by side).</p>
<p>Note: If you resize the browser window, the links will automatically break when it becomes too 

crowded.</p>

<ul class="nav">
  <li><a href="#home">Home</a></li>
  <li><a href="#about">About Us</a></li>
  <li><a href="#clients">Our Clients</a></li>  
  <li><a href="#contact">Contact Us</a></li>
</ul>

</body>
</html>

<kbd>return</kbd>[Back to table of contents](#homepage)


--------


## CSS Combinators

The relationship between the selectors in an HTML page is explained by combinators.

More than one single selector can be contained in a CSS selector, and we can include a combinator between 

simple selectors. The four unique combinators, and their representation (in parenthesis) in CSS include:



    descendant selector (space)
    child selector (>)
    adjacent sibling selector (+)
    general sibling selector (~)



Descendant Selector  ( );

Descendant selector matches all the elements that are descendants of the same specified element. It is 

specified using empty space. For example, in the code below, the <p> elements that are inside the <div> 

elements are selected:


<!DOCTYPE html>
<html>
<head>
<style>
div p {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>Descendant Selector</h2>
<p>The descendant selector matches all elements that are descendants of a specified element.</p>

<div>
  <p>Paragraph 1 in the div.</p>
  <p>Paragraph 2 in the div.</p>
  <section><p>Paragraph 3 in the div.</p></section>
</div>

<p>Paragraph 4. Not in a div.</p>
<p>Paragraph 5. Not in a div.</p>

</body>
</html>


Child Selector (>)

Child selector selects all elements that are the children of a specified element. It is denoted using the 

greater than symbol. In the code below for example, all the <p> elements that are children of a <div> 

element are selected:



<!DOCTYPE html>
<html>
<head>
<style>
div > p {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>Child Selector</h2>
<p>The child selector (>) selects all elements that are the children of a specified element.</p>

<div>
  <p>Paragraph 1 in the div.</p>
  <p>Paragraph 2 in the div.</p>
  <section><p>Paragraph 3 in the div.</p></section> <!-- not Child but Descendant -->
  <p>Paragraph 4 in the div.</p>
</div>

<p>Paragraph 5. Not in a div.</p>
<p>Paragraph 6. Not in a div.</p>

</body>
</html>



Note that elements not directly under a parent but have a sub-parent is a descendant not a child of another.




Adjacent Sibling Selector (+);


The adjacent sibling selector is used to select an element that is located after another specific element. 

Here adjacent means "immediately following". Sibling elements must have same parent. The adjacent sibling 

selector is denoted with the plus (+) sign. In the example below, only the first <p> elements that are 

placed "immediately" after <div> elements are selected.

<!DOCTYPE html>
<html>
<head>
<style>
div + p {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>Adjacent Sibling Selector</h2>

<p>The + selector is used to select an element that is directly after another specific element.</p>
<p>The following example selects the first p element that are placed immediately after div elements:</p>

<div>
  <p>Paragraph 1 in the div.</p>
  <p>Paragraph 2 in the div.</p>
</div>

<p>Paragraph 3. After a div.</p>
<p>Paragraph 4. After a div.</p>

<div>
  <p>Paragraph 5 in the div.</p>
  <p>Paragraph 6 in the div.</p>
</div>

<p>Paragraph 7. After a div.</p>
<p>Paragraph 8. After a div.</p>

</body>
</html>


General Sibling Selector (~);

The general sibling selector selects 'all' elements that are "next siblings" of a specified element. It is 

denoted by tilda sign (~). Remember that all elements in the body are siblings of <html>. In the example 

below, all the <p> elements that are next siblings of <div> elements are selected:



<!DOCTYPE html>
<html>
<head>
<style>
div ~ p {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>General Sibling Selector</h2>
<p>The general sibling selector (~) selects all elements that are next siblings of a specified element.</p>

<p>Paragraph 1.</p>

<div>
  <p>Paragraph 2.</p>
</div>

<p>Paragraph 3.</p>
<code>Some code.</code>
<p>Paragraph 4.</p>

</body>
</html>


All CSS Combinator Selectors
Selector 	Example 	Example description
element element 	div p 	Selects all <p> elements inside <div> elements
element>element 	div > p 	Selects all <p> elements where the parent is a <div> element
element+element 	div + p 	Selects the first <p> element that are placed immediately after 

<div> elements
element1~element2 	p ~ ul 	Selects every <ul> element that are preceded by a <p> element


<kbd>return</kbd>[Back to table of contents](#homepage)


-------



## CSS Pseudo-class

A pseudo-class is used to define a special state of an element. For instance, you can use psedo-class to 

style:

-an element when a user mouses over it
-visited and unvisited links differently
-an element when it gets focus


The general syntax for pseudo-classes is:

selector:pseudo-class {
  property: value;
}

alternatively, you can specify the class of the selector.

selector.class:pseudo-class {
  property: value;
}





Anchor Pseudo-classes;

They are used to display links in different ways.See illustration below for some ways links can be displayed 

based on the action of mouse on it (visited, hovered on, unvisited, during click):


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


Note: a:hover MUST come after a:link and a:visited in the CSS definition in order to be effective! a:active 

MUST come after a:hover in the CSS definition in order to be effective! Pseudo-class names are not case-

sensitive.



Pseudo-classes and CSS Classes;

Pseudo-classes can be combined with CSS classes. This enables a specific application of pseudo classes to 

elements. In the example below, hovering over the link will make the link change color:


<!DOCTYPE html>
<html>
<head>
<style>
a.highlight:hover {
  color: #ff0000;
} 
</style>
</head>
<body>

<h2>Pseudo-classes and CSS Classes</h2>
<p>When you hover over the first link below, it will change color:</p>

<p><a class="highlight" href="css_syntax.asp">CSS Syntax</a></p>
<p><a href="default.asp">CSS Tutorial</a></p>

</body>
</html>




Hover on <div>;

The example below shows how to use :hover pseudo-class on a <div> element:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: green;
  color: white;
  padding: 25px;
  text-align: center;
}

div:hover {
  background-color: blue;
}
</style>
</head>
<body>

<p>Mouse over the div element below to change its background color:</p>

<div>Mouse Over Me</div>

</body>
</html>



Simple Tooltip Hover;

This enables you to show a <p> element(like a tooltip) by hovering over a <div> element. You can also use it 

for other selectors. See illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
p {
  display: none;
  background-color: yellow;
  padding: 20px;
}

div:hover p {
  display: block;
}
</style>
</head>
<body>

<div>Hover over me to show the p element
  <p>Tada! Here I am!</p>
</div>

</body>
</html>



CSS - The :first-child Pseudo-class

The :first-child pseudo-class matches a specified element that is the first child of another element. 


Match the first <p> element::

In the example below, the selector matches any <p> element that is the first child of any element:



<!DOCTYPE html>
<html>
<head>
<style>
p:first-child {
  color: blue;
} 
</style>
</head>
<body>

<p>This is some text.</p>
<p>This is some text.</p>

</body>
</html>



Match the first <i> element in all <p> elements::

In the example below, the selector matches the first <i> element in all <p> elements:

<!DOCTYPE html>
<html>
<head>
<style>
p i:first-child {
  color: blue;
} 
</style>
</head>
<body>

<p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
<p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>

</body>
</html>



Match all <i> elements in all first child <p> elements::

In the example below, the selector matches all <i> elements in <p> elements which are first child of another 

element:


<!DOCTYPE html>
<html>
<head>
<style>
p:first-child i {
  color: blue;
} 
</style>
</head>
<body>

<p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
<p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>

</body>
</html>


CSS - The :lang Pseudo-class::

The :lang pseudo class allows you to define special rules for different languages. The :lang in the example 

below defines the quotations marks for <q> elements with lang= "no" (the quotation mark used in this case is 

~text here~:


<!DOCTYPE html>
<html>
<head>
<style>
q:lang(no) {
  quotes: "~" "~";
}
</style>
</head>
<body>

<p>Some text <q lang="no">A quote in a paragraph</q> Some text.</p>
<p>In this example, :lang defines the quotation marks for q elements with lang="no":</p>

</body>
</html>


Some Additional Examples of Pseudo Class::

Adding different styles to hyperlinks:::

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

<h2>Styling Links</h2>

<p>Mouse over the links and watch them change layout:</p>

<p><b><a class="one" href="default.asp" target="_blank">This link changes color</a></b></p>
<p><b><a class="two" href="default.asp" target="_blank">This link changes font-size</a></b></p>
<p><b><a class="three" href="default.asp" target="_blank">This link changes background-color</a></b></p>
<p><b><a class="four" href="default.asp" target="_blank">This link changes font-family</a></b></p>
<p><b><a class="five" href="default.asp" target="_blank">This link changes text-decoration</a></b></p>

</body>
</html>



Use of focus:::

The :focus pseudo-class is used to style the part of a page while work is being done on it. For example, you 

may define a specific style, using pseudo-class, for a Form bar in focus (currently being filled):


<!DOCTYPE html>
<html>
<head>
<style>
input:focus {
  background-color: yellow;
}
</style>
</head>
<body>

<form action="/action_page.php" method="get">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>





Here are additional Pseudo-classes and tips to help in their usage:



All CSS Pseudo Classes

Selector 	Example 	Example description
:active 	a:active 	Selects the active link
:checked 	input:checked 	Selects every checked <input> element
:disabled 	input:disabled 	Selects every disabled <input> element
:empty 	p:empty 	Selects every <p> element that has no children
:enabled 	input:enabled 	Selects every enabled <input> element
:first-child 	p:first-child 	Selects every <p> elements that is the first child of its parent
:first-of-type 	p:first-of-type 	Selects every <p> element that is the first <p> element of its 

parent
:focus 	input:focus 	Selects the <input> element that has focus
:hover 	a:hover 	Selects links on mouse over
:in-range 	input:in-range 	Selects <input> elements with a value within a specified range
:invalid 	input:invalid 	Selects all <input> elements with an invalid value
:lang(language) 	p:lang(it) 	Selects every <p> element with a lang attribute value starting with 

"it"
:last-child 	p:last-child 	Selects every <p> elements that is the last child of its parent
:last-of-type 	p:last-of-type 	Selects every <p> element that is the last <p> element of its parent
:link 	a:link 	Selects all unvisited links
:not(selector) 	:not(p) 	Selects every element that is not a <p> element
:nth-child(n) 	p:nth-child(2) 	Selects every <p> element that is the second child of its parent
:nth-last-child(n) 	p:nth-last-child(2) 	Selects every <p> element that is the second child of its 

parent, counting from the last child
:nth-last-of-type(n) 	p:nth-last-of-type(2) 	Selects every <p> element that is the second <p> element of 

its parent, counting from the last child
:nth-of-type(n) 	p:nth-of-type(2) 	Selects every <p> element that is the second <p> element of 

its parent
:only-of-type 	p:only-of-type 	Selects every <p> element that is the only <p> element of its parent
:only-child 	p:only-child 	Selects every <p> element that is the only child of its parent
:optional 	input:optional 	Selects <input> elements with no "required" attribute
:out-of-range 	input:out-of-range 	Selects <input> elements with a value outside a specified range
:read-only 	input:read-only 	Selects <input> elements with a "readonly" attribute specified
:read-write 	input:read-write 	Selects <input> elements with no "readonly" attribute
:required 	input:required 	Selects <input> elements with a "required" attribute specified
:root 	root 	Selects the document's root element
:target 	#news:target 	Selects the current active #news element (clicked on a URL containing that 

anchor name)
:valid 	input:valid 	Selects all <input> elements with a valid value
:visited 	a:visited 	Selects all visited links



All CSS Pseudo Elements

Selector 	Example 	Example description
::after 	p::after 	Insert content after every <p> element
::before 	p::before 	Insert content before every <p> element
::first-letter 	p::first-letter 	Selects the first letter of every <p> element
::first-line 	p::first-line 	Selects the first line of every <p> element
::selection 	p::selection 	Selects the portion of an element that is selected by a user

<kbd>return</kbd>[Back to table of contents](#homepage)



----------


## CSS Pseudo-element

A CSS pseudo-element is used to style specific parts of an element such as: 
Styling the first letter, or line of an element; or 
Inserting content befor, or after, the content of another element. 



The syntax of pseudo-elements is:

selector::pseudo-element {
  property: value;
}




The ::first-line Pseudo-element ;;

The ::first-line pseudo-element is used to add a special style to the first line of a text. In the example 

below, the first line of text in all <p> elements is formatted:


<!DOCTYPE html>
<html>
<head>
<style>
p::first-line {
  color: #ff0000;
  font-variant: small-caps;
}
</style>
</head>
<body>

<p>You can use the ::first-line pseudo-element to add a special effect to the first line of a text. Some 

more text. And even more, and more, and more, and more, and more, and more, and more, and more, and more, 

and more, and more, and more.</p>

</body>
</html>


Please note that the ::first-line  pseudo-element can only be applied to block level elements. The following 

properties apply to the ::first-line pseudo-element:font properties, color properties, background 

properties, word-spacing, letter-spacing, text-decoration, vertical-align, text-transform, and line-height, 

clear.

The double colon notation of ::first-line is the standard used in CSS3 (unlike CSS 1 and 2 where single 

colon was used i.e. :first-line). This helps distinguish between pseudo-elements and pseudo-classes. For 

backward compatibility, the single-color syntax is acceptable in CSS2 and CSS1 pseudo-elements. 




The ::first-letter Pseudo-element ;;

The ::first-letter pseudo-element is used to add a special style to the first letter of a text. The example 

below shows how to use ::first-letter pseudo element to format the first letter of the text in all <p> 

elements:

<!DOCTYPE html>
<html>
<head>
<style>
p::first-letter {
  color: #ff0000;
  font-size: xx-large;
}
</style>
</head>
<body>

<p>You can use the ::first-letter pseudo-element to add a special effect to the first character of a text!

</p>

</body>
</html>



Note that: The ::first-letter pseudo element can only be applied to block-level elements. The following 

properties apply to the ::first-letter pseudo-element:font properties, color properties, background 

properties, margin properties, padding properties, border properties, text-decoration, vertical-align (only 

if "float" is "none"), text-transform, line-height, float, and clear.



Pseudo-elements and CSS Classes::

The Pseudo-elements can also be combined with CSS classes. This ensures that you can select a specific <p> 

element rather than apply pseudo-element styling to all <p> elements. In this case, the first letter of 

paragraphs with class="intro" will be displayed in red and in larger size. See illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
p.intro::first-letter {
  color: #ff0000;
  font-size: 200%;
}  
</style>
</head>
<body>

<p class="intro">This is an introduction.</p>
<p>This is a paragraph with some text. A bit more text even.</p>

</body>
</html>


Multiple Pseudo-elements::

Several pseudo-elements can also be combined. In the example below, the first letter of a paragraph will be 

red, in an XX-large font size. The rest of the first line will be blue, and in small-caps. The rest of the 

paragraph will be the default font size and color. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
p::first-letter {
  color: #ff0000;
  font-size: xx-large;
}

p::first-line {
  color: #0000ff;
  font-variant: small-caps;
}
</style>
</head>
<body>

<p>You can combine the ::first-letter and ::first-line pseudo-elements to add a special effect to the first 

letter and the first line of a text!</p>

</body>
</html>



CSS - The ::before Pseudo-element::

The ::before pseudo-element can be used to insert some content before the content of an element. In the 

example below, and image (smiley.gif) is inserted before the content of each <h1> element:


<!DOCTYPE html>
<html>
<head>
<style>
h1::before {
  content: url(smiley.gif);
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>The ::before pseudo-element inserts content before the content of an element.</p>

<h1>This is a heading</h1>

</body>
</html>




CSS - The ::after Pseudo-element


The ::after pseudo-element can be used to insert some content after the content of an element. The example 

below shows the insertion of an image after the content of each <h1> element:


<!DOCTYPE html>
<html>
<head>
<style>
h1::after {
  content: url(smiley.gif);
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>The ::after pseudo-element inserts content after the content of an element.</p>

<h1>This is a heading</h1>

</body>
</html>



CSS - The ::marker Pseudo-element

The ::marker pseudo-element selects (styles) the markers of list of items. The example below shows styling 

of markers of list of items using ::marker pseudo-element:


<!DOCTYPE html>
<html>
<head>
<style>
::marker { 
  color: red;
  font-size: 23px;
}
</style>
</head>
<body>

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<ol>
  <li>First</li>
  <li>Second</li>
  <li>Third</li>
</ol>

</body>
</html>


NB: You don't have to style based on class here, the ::marker style will apply to all markers. 




CSS - The ::selection Pseudo-element::


The ::selection pseudo-element matches the portion of an element that is selected by a user. The properties 

that can be applied to ::selection include: color, background, cursor, and outline. The styling in the 

example below makes a selected text red on a yellow background:


<!DOCTYPE html>
<html>
<head>
<style>
::-moz-selection { /* Code for Firefox */
  color: red;
  background: yellow;
}

::selection {
  color: red;
  background: yellow;
}
</style>
</head>
<body>

<h1>Select some text on this page:</h1>

<p>This is a paragraph.</p>
<div>This is some text in a div element.</div>

<p><strong>Note:</strong> Firefox supports an alternative, the ::-moz-selection property.</p>

</body>
</html>




All CSS Pseudo Elements
Selector 	Example 	Example description
::after 	p::after 	Insert something after the content of each <p> element
::before 	p::before 	Insert something before the content of each <p> element
::first-letter 	p::first-letter 	Selects the first letter of each <p> element
::first-line 	p::first-line 	Selects the first line of each <p> element
::marker 	::marker 	Selects the markers of list items
::selection 	p::selection 	Selects the portion of an element that is selected by a user
All CSS Pseudo Classes
Selector 	Example 	Example description
:active 	a:active 	Selects the active link
:checked 	input:checked 	Selects every checked <input> element
:disabled 	input:disabled 	Selects every disabled <input> element
:empty 	p:empty 	Selects every <p> element that has no children
:enabled 	input:enabled 	Selects every enabled <input> element
:first-child 	p:first-child 	Selects every <p> elements that is the first child of its parent
:first-of-type 	p:first-of-type 	Selects every <p> element that is the first <p> element of its 

parent
:focus 	input:focus 	Selects the <input> element that has focus
:hover 	a:hover 	Selects links on mouse over
:in-range 	input:in-range 	Selects <input> elements with a value within a specified range
:invalid 	input:invalid 	Selects all <input> elements with an invalid value
:lang(language) 	p:lang(it) 	Selects every <p> element with a lang attribute value starting with 

"it"
:last-child 	p:last-child 	Selects every <p> elements that is the last child of its parent
:last-of-type 	p:last-of-type 	Selects every <p> element that is the last <p> element of its parent
:link 	a:link 	Selects all unvisited links
:not(selector) 	:not(p) 	Selects every element that is not a <p> element
:nth-child(n) 	p:nth-child(2) 	Selects every <p> element that is the second child of its parent
:nth-last-child(n) 	p:nth-last-child(2) 	Selects every <p> element that is the second child of its 

parent, counting from the last child
:nth-last-of-type(n) 	p:nth-last-of-type(2) 	Selects every <p> element that is the second <p> element of 

its parent, counting from the last child
:nth-of-type(n) 	p:nth-of-type(2) 	Selects every <p> element that is the second <p> element of 

its parent
:only-of-type 	p:only-of-type 	Selects every <p> element that is the only <p> element of its parent
:only-child 	p:only-child 	Selects every <p> element that is the only child of its parent
:optional 	input:optional 	Selects <input> elements with no "required" attribute
:out-of-range 	input:out-of-range 	Selects <input> elements with a value outside a specified range
:read-only 	input:read-only 	Selects <input> elements with a "readonly" attribute specified
:read-write 	input:read-write 	Selects <input> elements with no "readonly" attribute
:required 	input:required 	Selects <input> elements with a "required" attribute specified
:root 	root 	Selects the document's root element
:target 	#news:target 	Selects the current active #news element (clicked on a URL containing that 

anchor name)
:valid 	input:valid 	Selects all <input> elements with a valid value
:visited 	a:visited 	Selects all visited links


<kbd>return</kbd>[Back to table of contents](#homepage)



----------



## CSS Opacity


The opacity property quantifies the opacity or trasparency of an element.\


Transparent Image
Opacity of an image ranges from 0 to 1, with 0 being fully transparent and 1.0 meaning fully opaque. See 

example code below:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  opacity: 0.5;
}
</style>
</head>
<body>

<h1>Image Transparency</h1>
<p>The opacity property specifies the transparency of an element. The lower the value, the more 

transparent:</p>

<p>Image with 50% opacity:</p>
<img src="img_forest.jpg" alt="Forest" width="170" height="100">

</body>
</html>



Transparent Hover Effect

It is common for opacity property to be used alongside :hover selector to change the opacity of an image on 

mouse-over. See illustration of how to modify opacity of an image on mouseover below:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  opacity: 0.5;
}

img:hover {
  opacity: 1.0;
}
</style>
</head>
<body>

<h1>Image Transparency</h1>
<p>The opacity property is often used together with the :hover selector to change the opacity on mouse-

over:</p>
<img src="img_forest.jpg" alt="Forest" width="170" height="100">
<img src="img_mountains.jpg" alt="Mountains" width="170" height="100">
<img src="img_5terre.jpg" alt="Italy" width="170" height="100">

</body>
</html>



Note on example above: The CSS style shows what happens when a user hovers over one of the images. And in 

this example, we want the image to NOT be transparent when user mouses-over it. The CSS for this is thus 

opacity:1; upon hovering, and the pseudo class is set accordingly. 




Transparent Box

The opacity property used in adding transparency to an element is also inherited by the child elements. This 

can make text too transparent to be readable. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #4CAF50;
  padding: 10px;
}

div.first {
  opacity: 0.1;
}

div.second {
  opacity: 0.3;
}

div.third {
  opacity: 0.6;
}
</style>
</head>
<body>

<h1>Transparent Box</h1>
<p>When using the opacity property to add transparency to the background of an element, all of its child 

elements become transparent as well. This can make the text inside a fully transparent element hard to 

read:</p>

<div class="first"><p>opacity 0.1</p></div>
<div class="second"><p>opacity 0.3</p></div>
<div class="third"><p>opacity 0.6</p></div>
<div><p>opacity 1 (default)</p></div>

</body>
</html>


Transparency using RGBA:::

The use of RGBA prevents the application of opacity to child elements. Once you specify color as RGBA, the 

opacity is only set for the background color and not the text. 

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background: rgb(76, 175, 80);
  padding: 10px;
}

div.first {
  background: rgba(76, 175, 80, 0.1);
}

div.second {
  background: rgba(76, 175, 80, 0.3);
}

div.third {
  background: rgba(76, 175, 80, 0.6);
}
</style>
</head>
<body>

<h1>Transparent Box</h1>
<p>With opacity:</p>
<div style="opacity:0.1;"><p>10% opacity</p></div>
<div style="opacity:0.3;"><p>30% opacity</p></div>
<div style="opacity:0.6;"><p>60% opacity</p></div>
<div><p>opacity 1</p></div>

<p>With RGBA color values:</p>
<div class="first"><p>10% opacity</p></div>
<div class="second"><p>30% opacity</p></div>
<div class="third"><p>60% opacity</p></div>
<div><p>default</p></div>

<p>Notice how the text gets transparent as well as the background color when using the opacity property.</p>

</body>
</html>


Text in Transparent Box:::

In CSS, we can also create text in transparent box. The process involves: First, creating a <div> element 

(class="background") with a background image, and a border.

Then we create another <div> (class="transbox") inside the first <div>.

The <div class="transbox"> have a background color, and a border - the div is transparent.

Inside the transparent <div>, we add some text inside a <p> element. The example below shows how to insert 

text inside a transparent box:
 

<!DOCTYPE html>
<html>
<head>
<style>
div.background {
  background: url(klematis.jpg) repeat;
  border: 2px solid black;
}

div.transbox {
  margin: 30px;
  background-color: #ffffff;
  border: 1px solid black;
  opacity: 0.6;
}

div.transbox p {
  margin: 5%;
  font-weight: bold;
  color: #000000;
}
</style>
</head>
<body>

<div class="background">
  <div class="transbox">
    <p>This is some text that is placed in the transparent box.</p>
  </div>
</div>

</body>
</html>


<kbd>return</kbd>[Back to table of contents](#homepage)
