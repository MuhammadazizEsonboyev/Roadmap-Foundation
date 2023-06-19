## HTML CHARSET
HTML charset attribute:
To display an HTML page correctly, a web browser must know the character set used in the page. 

```
<meta charset="UTF-8">
```
if you do not specify the charset, "UTF-8" is the default in HTML.


UTF-8 Characters: You can't type them on the keyboard but they can always be displayed using numbers ( entity numbers)

* Both ```<p>``` in the paragraph below are the same
```
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
</head>
<body>

<p>I will display A B C</p>
<p>I will display &#65; &#66; &#67;</p>

</body>
</html> 
```
* A, B, C are 65, 66, and 67 respectively

To let browser recognize that you are displaying a utf-8 character, you must start with &# and end it with a semi-colon (;)

Emojis are also characters from utf-8.

* You can size emojis like other characters
```
<p style="font-size:48px">
&#128512; &#128516; &#128525; &#128151;
</p>
```
* HTML Encoding ( Character sets)

A browser must know the character set to use to display it correctly. 

** Excerpts from the HTML ENCODING CHAPTER
From ASCII to UTF-8

ASCII was the first character encoding standard. ASCII defined 128 different characters that could be used on the internet: numbers (0-9), English letters (A-Z), and some special characters like ! $ + - ( ) @ < > .

ISO-8859-1 was the default character set for HTML 4. This character set supported 256 different character codes. HTML 4 also supported UTF-8.

ANSI (Windows-1252) was the original Windows character set. ANSI is identical to ISO-8859-1, except that ANSI has 32 extra characters.

The HTML5 specification encourages web developers to use the UTF-8 character set, which covers almost all of the characters and symbols in the world!

** HTML charset attribute
you specify it in the <meta> tag of the HTML page.

```
<meta charset="UTF-8">
```
<kbd>return</kbd>[Back to table of contents](#homepage)


-------



## HTML Forms

* Filling a form that contains user name and password and that redirects the form to a specific page after servers process the input.
```
<h2>HTML Forms</h2>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 

<p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>
```

* The ```<form>``` Element

The HTML ```<form>``` element is used to create an HTML form for user input:
```
<form>

form elements

</form>
```

The form element is like a container for all kinds of  input elements like: text fields, checkboxes, radio buttons, submit buttons, etc.


* The ```<input>``` element: is the most used form element and can be displayed on the 'type' attribute. 
```
Type 	Description
<input type="text"> 	Displays a single-line text input field
<input type="radio"> 	Displays a radio button (for selecting one of many choices)
<input type="checkbox"> 	Displays a checkbox (for selecting zero or more of many choices)
<input type="submit"> 	Displays a submit button (for submitting the form)
<input type="button"> 	Displays a clickable button
```

* Text Fields: ```<input type="text"> ```

This defines a single-line input field for text input. The form itself is not visible and the number of characters is by default 20 characters. 
```
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form> 
```
The ```<label>``` tag defines a label for many form elements.

The ```<label>``` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focus on the input element.

The ```<label>``` element also help users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the ```<label>``` element, it toggles the radio button/checkbox.

The for attribute of the ```<label>``` tag should be equal to the id attribute of the <input> element to bind them together. 


* Radio Buttons
```
<input type="radio"> defines the radio button which lets use select ONLY one among a few choices.
```
* see sample radio buttons below:
```
<form>
  <input type="radio" id="male" name="gender" value="male">
  <label for="male">Male</label><br>
  <input type="radio" id="female" name="gender" value="female">
  <label for="female">Female</label><br>
  <input type="radio" id="other" name="gender" value="other">
  <label for="other">Other</label>
</form> 
```

* Checkboxes: Enables users select zero or more among a limited no of choices 
```
<input type="checkbox"> defines a checkbox
```
NB: the value attribute  can indicate the default option
 
* See example of form below:
```
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form> 
```

* The Submit Button
```
<input type="submit"> defines the button for submitting form data to a form-handler. 
```
Example of a form with a submit button below: 
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 
```

* he Name Attribute for ```<input>```
* Each input field must have a name to be submitted. If the value of the name attribute is omitted, the input field value will not be sent at all. 

<kbd>return</kbd>[Back to table of contents](#homepage)

## HTML Form Attributes

* The HTML Form Attribute: A discussion of different attributes

The Action Attribute: defines action to be performed when form is submitted.  Form data is usually sent to a file on  server when submit button is clicked. If you omit action attribute, the action is set to the current page.

* To send form data to a file called action_page.php containing a server-side script that handles the form data:
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 
```

* The Target Attribute
This specified where to display response received after submitting the form. 

See below for the possible values of the target attribute

Value 	Description
```
_blank 	The response is displayed in a new window or tab
_self 	The response is displayed in the current window (default)
_parent 	The response is displayed in the parent frame
_top 	The response is displayed in the full body of the window
framename 	The response is displayed in a named iframe
```
* Example of the use of target attribute:
```
<p>When submitting this form, the result will be opened in a new browser tab:</p>

<form action="/action_page.php" target="_blank">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 
```

* The Method Attribute

This specifies the method attribute specifies HTTP method used when submitting form data. 

* The get method: ```<form action="/action_page.php" method="get"> ```
* The post method:  ```<form action="/action_page.php" method="post"> ```

* Tip: Always use POST if the form data contains sensitive or personal information!

Notes on GET:
Appends the form data to the URL, in name/value pairs
NEVER use GET to send sensitive data! (the submitted form data is visible in the URL!)
The length of a URL is limited (2048 characters)
Useful for form submissions where a user wants to bookmark the result
GET is good for non-secure data, like query strings in Google

Notes on POST:
Appends the form data inside the body of the HTTP request (the submitted form data is not shown in the URL)
POST has no size limitations, and can be used to send large amounts of data.
Form submissions with POST cannot be bookmarked

Tip: Always use POST if the form data contains sensitive or personal information!

* The Autocomplete Attribute
Specifies whether a form should have autocomplete on or off. Autocomplete when left on enables browser automatically complete values based on previously entered values in the same browser. 
```
<form action="/action_page.php" autocomplete="on"> 
```

The Novalidate Attribute
This is a boolean attribute which specifies form-data (input) should not be validated when submitted. 
```
<form action="/action_page.php" novalidate> 
```
* List of All <form> Attributes

```
Attribute 	Description
accept-charset 	Specifies the character encodings used for form submission
action 	Specifies where to send the form-data when a form is submitted
autocomplete 	Specifies whether a form should have autocomplete on or off
enctype 	Specifies how the form-data should be encoded when submitting it to the server (only for method="post")
method 	Specifies the HTTP method to use when sending form-data
name 	Specifies the name of the form
novalidate 	Specifies that the form should not be validated when submitted
rel 	Specifies the relationship between a linked resource and the current document
target 	Specifies where to display the response that is received after submitting the form
```
<kbd>return</kbd>[Back to table of contents](#homepage)


------



## HTML Form Attributes

* The HTML Form Attribute: A discussion of different attributes

The Action Attribute: defines action to be performed when form is submitted.  Form data is usually sent to a file on  server when submit button is clicked. If you omit action attribute, the action is set to the current page.

* To send form data to a file called action_page.php containing a server-side script that handles the form data:
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 
```

* The Target Attribute
This specified where to display response received after submitting the form. 

See below for the possible values of the target attribute

Value 	Description
```
_blank 	The response is displayed in a new window or tab
_self 	The response is displayed in the current window (default)
_parent 	The response is displayed in the parent frame
_top 	The response is displayed in the full body of the window
framename 	The response is displayed in a named iframe
```
* Example of the use of target attribute:
```
<p>When submitting this form, the result will be opened in a new browser tab:</p>

<form action="/action_page.php" target="_blank">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 
```

* The Method Attribute

This specifies the method attribute specifies HTTP method used when submitting form data. 

* The get method: ```<form action="/action_page.php" method="get"> ```
* The post method:  ```<form action="/action_page.php" method="post"> ```

* Tip: Always use POST if the form data contains sensitive or personal information!

Notes on GET:
Appends the form data to the URL, in name/value pairs
NEVER use GET to send sensitive data! (the submitted form data is visible in the URL!)
The length of a URL is limited (2048 characters)
Useful for form submissions where a user wants to bookmark the result
GET is good for non-secure data, like query strings in Google

Notes on POST:
Appends the form data inside the body of the HTTP request (the submitted form data is not shown in the URL)
POST has no size limitations, and can be used to send large amounts of data.
Form submissions with POST cannot be bookmarked

Tip: Always use POST if the form data contains sensitive or personal information!

* The Autocomplete Attribute
Specifies whether a form should have autocomplete on or off. Autocomplete when left on enables browser automatically complete values based on previously entered values in the same browser. 
```
<form action="/action_page.php" autocomplete="on"> 
```

The Novalidate Attribute
This is a boolean attribute which specifies form-data (input) should not be validated when submitted. 
```
<form action="/action_page.php" novalidate> 
```
* List of All <form> Attributes

```
Attribute 	Description
accept-charset 	Specifies the character encodings used for form submission
action 	Specifies where to send the form-data when a form is submitted
autocomplete 	Specifies whether a form should have autocomplete on or off
enctype 	Specifies how the form-data should be encoded when submitting it to the server (only for method="post")
method 	Specifies the HTTP method to use when sending form-data
name 	Specifies the name of the form
novalidate 	Specifies that the form should not be validated when submitted
rel 	Specifies the relationship between a linked resource and the current document
target 	Specifies where to display the response that is received after submitting the form
```
<kbd>return</kbd>[Back to table of contents](#homepage)


--------


## HTML Form Elements
HTML ```<form>``` Elements

The HTML <form> element can contain one or more of the following form elements:

```
<input>
<label>
<select>
<textarea>
<button>
<fieldset>
<legend>
<datalist>
<output>
<option>
<optgroup>
```

* The ```<input>``` Element
Input element is one of the most used form element. Can be displayed in varying ways depending on the type attribute
```
<label for="fname">First name:</label>
<input type="text" id="fname" name="fname"> 
```
* The ```<label>``` Element

```<label>``` element defines a label for several form elements. Helps screen-readers  read out the label when the user focus on the input. 
It also helps users click on text next to small regions ( like checkboxes and buttons)  to click those small areas. 

The 'for' attribute of the```<label>``` tag should equal to the 'id' attribute of the <input> element to bind them together.

* The ```<select>``` Element 

This element defvines a drop-down list:
```
<label for="cars">Choose a car:</label>
<select id="cars" name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select> 
```
* The option elements defines an option that can be selected. The first item is selected by default. Add the 'selected' attribute to an option to make it pre-selected. 
```
<option value="fiat" selected>Fiat</option> 
```
* Visible Values: Use size attribute to specify the number of visible values (a small scroll bar is inserted if you have more than the visible value set)
```
<label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="3">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select> 
```

* Allow Multiple Selections: 'multiple' attribute allow user to select more than one value. To use this, you have to Hold down the Ctrl (windows) / Command (Mac) button to select multiple options
```
<label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="4" multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select> 
```

* The ```<textarea>``` Element
The ```<textarea>``` element defines a multi-line input field (a text area):
The rows attribute specifies the visible number of lines in a text area.

The cols attribute specifies the visible width of a text area.

This is how the HTML code above will be displayed in a browser:
```
<textarea name="message" rows="10" cols="30">
The cat was playing in the garden.
</textarea> 
``` 
CSS can also be used to define the size of the text area. 
```
<textarea name="message" style="width:200px; height:600px;">
The cat was playing in the garden.
</textarea> 
```

* The ```<button>``` Element
Defines a clickable button.
```	
<button type="button" onclick="alert('Hello World!')">Click Me!</button>
```
Note: Always specify the type attribute for the button element. Different browsers may use different default types for the button element.

* The ```<fieldset>``` and ```<legend>``` Elements

The ```<fieldset>``` element is used to group related data in a form.

The ```<legend>``` element defines a caption for the <fieldset> element.

```
<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form> 
```

* The ```<datalist>``` Element
Specifies a list of pre-defined options for an ```<input>``` element (works like a kind of autocomplete which list options you can select from once you type a text) This should be usable with the normal form input element--experiment.

Users will see a drop-down list of the pre-defined options as they input data.

The list attribute of the ```<input>``` element, must refer to the id attribute of the <datalist> element

The datalist tag is not supported in Safari prior version 12.1
```
<form action="/action_page.php">
  <input list="browsers">
  <datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
</form> 
```

* The ```<output>``` Element
Rep the result of a calculation ( such as one performed by a script)
	
```
<form action="/action_page.php"
  oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  0
  <input type="range"  id="a" name="a" value="50">
  100 +
  <input type="number" id="b" name="b" value="50">
  =
  <output name="x" for="a b"></output>
  <br><br>
  <input type="submit">
</form> 
```

** HTML Form Elements
```
Tag 	Description
<form> 	Defines an HTML form for user input
<input> 	Defines an input control
<textarea> 	Defines a multiline input control (text area)
<label> 	Defines a label for an <input> element
<fieldset> 	Groups related elements in a form
<legend> 	Defines a caption for a <fieldset> element
<select> 	Defines a drop-down list
<optgroup> 	Defines a group of related options in a drop-down list
<option> 	Defines an option in a drop-down list
<button> 	Defines a clickable button
<datalist> 	Specifies a list of pre-defined options for input controls
<output> 	Defines the result of a calculation
```
<kbd>return</kbd>[Back to table of contents](#homepage)


------


## HTML Input Types
* HTML Input Types
The default is 'text'
```
<input type="button">
<input type="checkbox">
<input type="color">
<input type="date">
<input type="datetime-local">
<input type="email">
<input type="file">
<input type="hidden">
<input type="image">
<input type="month">
<input type="number">
<input type="password">
<input type="radio">
<input type="range">
<input type="reset">
<input type="search">
<input type="submit">
<input type="tel">
<input type="text">
<input type="time">
<input type="url">
<input type="week">
```
Tip: The default value of the type attribute is "text".


* Input Type Text(default width=20 characters)
```<input type="text">``` defines a single-line text input field:

```
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form> 
```

* Input Type Password
```
<input type="password"> defines a password field.The characters in a password field are masked (shown as asterisks or circles)

 <form>
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>
  <label for="pwd">Password:</label><br>
  <input type="password" id="pwd" name="pwd">
</form> 
```


* input  Type Submit
```<input type="submit">``` defines a button for submitting form data to a form-handler.

The form-handler is typically a server page with a script for processing input data.

The form-handler is specified in the form's action attribute:

If you omit the submit button's value attribute, the button will get a default text (typically 'Submit Query')
```
 <form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 
```

* Input Type Reset

```<input type="reset">``` defines a reset button that will reset all form values to their default values.: YOu can also add value attribute to the reset button to customize what shows up on the button.
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
  <input type="reset">
</form> 
```

* Input Type Radio
-Defines a radio button which lets a user select one of a limited number of choices:
```
<form>
  <input type="radio" id="male" name="gender" value="male">
  <label for="male">Male</label><br>
  <input type="radio" id="female" name="gender" value="female">
  <label for="female">Female</label><br>
  <input type="radio" id="other" name="gender" value="other">
  <label for="other">Other</label>
</form> 
```

* Input Type Checkbox

```<input type="checkbox">``` defines a checkbox.

Checkboxes let a user select ZERO or MORE options of a limited number of choices.
```
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form> 
```

* Input Type Button
```<input type="button">``` defines a button:

 ```<input type="button" onclick="alert('Hello World!')" value="Click Me!">``` 



* Input Type Color
The ```<input type="color">``` is used for input fields that should contain a color.

Depending on browser support, a color picker can show up in the input field.

type="color" is not supported in Internet Explorer 11 or Safari 9.1 (or earlier)

The value attribute defines a preselected value for the color.
```
<form>
  <label for="favcolor">Select your favorite color:</label>
  <input type="color" id="favcolor" name="favcolor" value="#ff0000">
  <input type="submit" value="Submit">
</form> 
```


* Input Type Date

The ```<input type="date">``` is used for input fields that should contain a date.

Depending on browser support, a date picker can show up in the input field.

type="date" is not supported in Safari or Internet Explorer 11 (or earlier)
```
<form>
  <label for="birthday">Birthday:</label>
  <input type="date" id="birthday" name="birthday">
  <input type="submit" value="Submit">
</form> 
```

You can also add 'min' and 'max' attributes to add restrictions to dates
```
<form action="/action_page.php">
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>
  
  <input type="submit" value="Submit">
</form>
```


* Input Type Datetime-local

The ```<input type="datetime-local">``` specifies a date and time input field, with no time zone.

Depending on browser support, a date picker can show up in the input field.
```
<form action="/action_page.php">
  <label for="birthdaytime">Birthday (date and time):</label>
  <input type="datetime-local" id="birthdaytime" name="birthdaytime">
  <input type="submit" value="Submit">
</form>
```

* Input Type Email

The ```<input type="email">``` is used for input fields that should contain an e-mail address.

Depending on browser support, the e-mail address can be automatically validated when submitted.

Some smartphones recognize the email type, and add ".com" to the keyboard to match email input

```
<form action="/action_page.php">
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email">
  <input type="submit" value="Submit">
</form>
```

* Input Type File
The ```<input type="file">``` defines a file-select field and a "Browse" button for file uploads.
```
<form action="/action_page.php">
  <label for="myfile">Select a file:</label>
  <input type="file" id="myfile" name="myfile"><br><br>
  <input type="submit" value="Submit">
</form>
```

* Input Type Month
The ```<input type="month">``` allows the user to select a month and year.

Depending on browser support, a date picker can show up in the input field.
```
<form action="/action_page.php">
  <label for="bdaymonth">Birthday (month and year):</label>
  <input type="month" id="bdaymonth" name="bdaymonth">
  <input type="submit" value="Submit">
</form>
```

* Input type Number
The ```<input type="number">``` defines a numeric input field.

You can also set restrictions on what numbers are accepted.

Typically adds up and down button to decrease and increase the values between the ranges

The following example displays a numeric input field, where you can enter a value from 1 to 5:
```
<form action="/action_page.php">
  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5">
  <input type="submit" value="Submit">
</form>
```


Input Restrictions

Here is a list of some common input restrictions:
Attribute 	Description
checked 	Specifies that an input field should be pre-selected when the page loads (for type="checkbox" or type="radio")
disabled 	Specifies that an input field should be disabled
max 	Specifies the maximum value for an input field
maxlength 	Specifies the maximum number of character for an input field
min 	Specifies the minimum value for an input field
pattern 	Specifies a regular expression to check the input value against
readonly 	Specifies that an input field is read only (cannot be changed)
required 	Specifies that an input field is required (must be filled out)
size 	Specifies the width (in characters) of an input field
step 	Specifies the legal number intervals for an input field
value 	Specifies the default value for an input field

You will learn more about input restrictions in the next chapter.

The following example displays a numeric input field, where you can enter a value from 0 to 100, in steps of 10. The default value is 30:
```
<form action="/action_page.php">
  <label for="quantity">Quantity:</label>
  <input type="number" id="quantity" name="quantity" min="0" max="100" step="10" value="30">
  <input type="submit" value="Submit">
</form>
```

* Input Type Range
The ```<input type="range">``` defines a control for entering a number whose exact value is not important (like a slider control). Default range is 0 to 100. However, you can set restrictions on what numbers are accepted with the min, max, and step attributes:
```
<form action="/action_page.php" method="get">
  <label for="vol">Volume (between 0 and 50):</label>
  <input type="range" id="vol" name="vol" min="0" max="50">
  <input type="submit" value="Submit">
</form>
```

* Input Type Search
```
<form action="/action_page.php">
  <label for="gsearch">Search Google:</label>
  <input type="search" id="gsearch" name="gsearch">
  <input type="submit" value="Submit">
</form>
```
* Input Type Search
The ```<input type="tel">``` is used for input fields that should contain a telephone number.
```
<form action="/action_page.php">
  <label for="phone">Enter a phone number:</label><br><br>
  <input type="tel" id="phone" name="phone" placeholder="123-45-678" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}" required><br><br>
  <small>Format: 123-45-678</small><br><br>
  <input type="submit" value="Submit">
</form>
```

* Input Type Time

The ```<input type="time">``` allows the user to select a time (no time zone).

Depending on browser support, a time picker can show up in the input field.If the browser supports it, a time picker pops up when entering the input field.
```
<form action="/action_page.php">
  <label for="appt">Select a time:</label>
  <input type="time" id="appt" name="appt">
  <input type="submit" value="Submit">
</form>
```

* Input Type Url

The ```<input type="url">``` is used for input fields that should contain a URL address.

Depending on browser support, the url field can be automatically validated when submitted.

Some smartphones recognize the url type, and adds ".com" to the keyboard to match url input.

```
<form action="/action_page.php">
  <label for="homepage">Add your homepage:</label>
  <input type="url" id="homepage" name="homepage">
  <input type="submit" value="Submit">
</form>
```
* Input Type Week
The ```<input type="week">``` allows the user to select a week and year.

Depending on browser support, a date picker can show up in the input field.If the browser supports it, a date picker pops up when entering the input field
```
<form action="/action_page.php">
  <label for="week">Select a week:</label>
  <input type="week" id="week" name="week">
  <input type="submit" value="Submit">
</form>
```
<kbd>return</kbd>[Back to table of contents](#homepage)

## HTML Input Attributes

HTML Input Type Attribute
Tag 	Description
```<input type="">``` 	Specifies the input type to display

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
HTML Input Attributes: Attributes of input element

* The value attribute
Specifies the initial(default) value for the imput field
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The readonly Attribute
Specifies an input field to be read-only. This input field cannot be modified  but user can tab into it, highlight, and copy text from it. The value is sent when submitting the form. 
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" readonly><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The disabled attribute
Specified that an input field is disabled, and such field is unusable and unclickable. Value will not be sent when submitting the form.
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" disabled><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The size Attribute

Specifies the visible width, in characters, of an input field. Default value is size 20. This attribute works with Text, search, tel, url, email, and password. 
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" size="4"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The maxlength Attribute

Specifies the maximum number of characters allowed in an input field. 

Note: When a maxlength is set, the input field will not accept more than the specified number of characters. However, this attribute does not provide any feedback. So, if you want to alert the user, you must write JavaScript code.

```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" maxlength="4" size="4"><br><br>
  <input type="submit" value="Submit">
</form>
```

* Min and Max Attribute
Specifies the min and max values for an input field. Works with number, range, date, datetime-local,month, time, and week. 

Tip: Use the max and min attributes together to create a range of legal values.
```
<form action="/action_page.php">
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>
  
  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5"><br><br>

  <input type="submit" value="Submit">
</form>
```

* The multiple Attribute
Specifies that the user is allowed to enter more than one value in an input field. multiple attribute works well with email and file types
```
<form action="/action_page.php">
  <label for="files">Select files:</label>
  <input type="file" id="files" name="files" multiple><br><br>
  <input type="submit" value="Submit">
</form>
```

* The pattern attribute

Specifies regular expressions that the input field's value is checked against when form is submitted. Pattern attribute works with text, date, search, url, tel, email, and password.

Tip: Use the global title attribute to describe the pattern to help the user.

Tip: Learn more about regular expressions in our JavaScript tutorial.

```
<form action="/action_page.php">
  <label for="country_code">Country code:</label>
  <input type="text" id="country_code" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The Placeholder Attribute
The input placeholder attribute specifies a short hint that describes the expected value of an input field (a sample value or a short description of the expected format).

The short hint is displayed in the input field before the user enters a value.

The placeholder attribute works with the following input types: text, search, url, tel, email, and password.
```
<form action="/action_page.php">
  <label for="phone">Enter a phone number:</label>
  <input type="tel" id="phone" name="phone" placeholder="123-45-678" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The required Attribute

Specifies that in input must be filled out before submitting the form. It works with the following input types: text, search, url, tel, email, passwork, date pickers, number, checkbox, radio, and file. 
```
<form action="/action_page.php">
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required>
  <input type="submit" value="Submit">
</form>
```


* he Step Attribute

Specifies legal number intervals for an input field (e.g. step="3" means that legal numbers could be -3, 0, 3, 6, etc.)

Tip: This attribute can be used together with the max and min attributes to create a range of legal values.

The step attribute works with the following input types: number, range, date, datetime-local, month, time and week.

```
<form action="/action_page.php">
  <label for="points">Points:</label>
  <input type="number" id="points" name="points" step="3">
  <input type="submit" value="Submit">
</form>
```
Note: Input restrictions are not foolproof, and JavaScript provides many ways to add illegal input. To safely restrict input, it must also be checked by the receiver (the server)!

* The Autofocus Attribute
The input autofocus attribute specifies the an input field automatically get focus when page loads.
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" autofocus><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The height and width Attributes

The input height and width attributes specify the height and width of an ```<input type="image">``` element.

Tip: Always specify both the height and width attributes for images. If height and width are set, the space required for the image is reserved when the page is loaded. Without these attributes, the browser does not know the size of the image, and cannot reserve the appropriate space to it. The effect will be that the page layout will change during loading (while the images load).
```
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
</form>
```
NB: The input ```type="image"``` sends the X and Y coordinates of the click that activated the image button


* The List Attribute
The input list attribute refers to a <datalist> element that contains pre-defined options for an <input> element.

```
<form action="/action_page.php">
  <input list="browsers" name="browser">
  <datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
  <input type="submit" value="Submit">
</form>
```

* The Autocomplete Attribute

The input autocomplete attribute specifies whether a form or an input field should have autocomplete on or off.

Autocomplete allows the browser to predict the value. When a user starts to type in a field, the browser should display options to fill in the field, based on earlier typed values.

The autocomplete attribute works with <form> and the following <input> types: text, search, url, tel, email, password, datepickers, range, and color.

In the case below, the autocomplete is on for the form but off for the email field. Fill in the form and reload to see the effect. 
```
<form action="/action_page.php" autocomplete="on">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" autocomplete="off"><br><br>
  <input type="submit" value="Submit">
</form>
```

* Use maxlength for no of characters: ```maxlength="40"``` 
And use max for numeric value, use max: ```max=40```

<kbd>return</kbd>[Back to table of contents](#homepage)


---------



## HTML Input Attributes

HTML Input Type Attribute
Tag 	Description
```<input type="">``` 	Specifies the input type to display

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
HTML Input Attributes: Attributes of input element

* The value attribute
Specifies the initial(default) value for the imput field
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The readonly Attribute
Specifies an input field to be read-only. This input field cannot be modified  but user can tab into it, highlight, and copy text from it. The value is sent when submitting the form. 
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" readonly><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The disabled attribute
Specified that an input field is disabled, and such field is unusable and unclickable. Value will not be sent when submitting the form.
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" disabled><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The size Attribute

Specifies the visible width, in characters, of an input field. Default value is size 20. This attribute works with Text, search, tel, url, email, and password. 
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" size="4"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The maxlength Attribute

Specifies the maximum number of characters allowed in an input field. 

Note: When a maxlength is set, the input field will not accept more than the specified number of characters. However, this attribute does not provide any feedback. So, if you want to alert the user, you must write JavaScript code.

```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" maxlength="4" size="4"><br><br>
  <input type="submit" value="Submit">
</form>
```

* Min and Max Attribute
Specifies the min and max values for an input field. Works with number, range, date, datetime-local,month, time, and week. 

Tip: Use the max and min attributes together to create a range of legal values.
```
<form action="/action_page.php">
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>
  
  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5"><br><br>

  <input type="submit" value="Submit">
</form>
```

* The multiple Attribute
Specifies that the user is allowed to enter more than one value in an input field. multiple attribute works well with email and file types
```
<form action="/action_page.php">
  <label for="files">Select files:</label>
  <input type="file" id="files" name="files" multiple><br><br>
  <input type="submit" value="Submit">
</form>
```

* The pattern attribute

Specifies regular expressions that the input field's value is checked against when form is submitted. Pattern attribute works with text, date, search, url, tel, email, and password.

Tip: Use the global title attribute to describe the pattern to help the user.

Tip: Learn more about regular expressions in our JavaScript tutorial.

```
<form action="/action_page.php">
  <label for="country_code">Country code:</label>
  <input type="text" id="country_code" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The Placeholder Attribute
The input placeholder attribute specifies a short hint that describes the expected value of an input field (a sample value or a short description of the expected format).

The short hint is displayed in the input field before the user enters a value.

The placeholder attribute works with the following input types: text, search, url, tel, email, and password.
```
<form action="/action_page.php">
  <label for="phone">Enter a phone number:</label>
  <input type="tel" id="phone" name="phone" placeholder="123-45-678" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The required Attribute

Specifies that in input must be filled out before submitting the form. It works with the following input types: text, search, url, tel, email, passwork, date pickers, number, checkbox, radio, and file. 
```
<form action="/action_page.php">
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required>
  <input type="submit" value="Submit">
</form>
```


* he Step Attribute

Specifies legal number intervals for an input field (e.g. step="3" means that legal numbers could be -3, 0, 3, 6, etc.)

Tip: This attribute can be used together with the max and min attributes to create a range of legal values.

The step attribute works with the following input types: number, range, date, datetime-local, month, time and week.

```
<form action="/action_page.php">
  <label for="points">Points:</label>
  <input type="number" id="points" name="points" step="3">
  <input type="submit" value="Submit">
</form>
```
Note: Input restrictions are not foolproof, and JavaScript provides many ways to add illegal input. To safely restrict input, it must also be checked by the receiver (the server)!

* The Autofocus Attribute
The input autofocus attribute specifies the an input field automatically get focus when page loads.
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" autofocus><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
</form>
```

* The height and width Attributes

The input height and width attributes specify the height and width of an ```<input type="image">``` element.

Tip: Always specify both the height and width attributes for images. If height and width are set, the space required for the image is reserved when the page is loaded. Without these attributes, the browser does not know the size of the image, and cannot reserve the appropriate space to it. The effect will be that the page layout will change during loading (while the images load).
```
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
</form>
```
NB: The input ```type="image"``` sends the X and Y coordinates of the click that activated the image button


* The List Attribute
The input list attribute refers to a <datalist> element that contains pre-defined options for an <input> element.

```
<form action="/action_page.php">
  <input list="browsers" name="browser">
  <datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
  <input type="submit" value="Submit">
</form>
```

* The Autocomplete Attribute

The input autocomplete attribute specifies whether a form or an input field should have autocomplete on or off.

Autocomplete allows the browser to predict the value. When a user starts to type in a field, the browser should display options to fill in the field, based on earlier typed values.

The autocomplete attribute works with <form> and the following <input> types: text, search, url, tel, email, password, datepickers, range, and color.

In the case below, the autocomplete is on for the form but off for the email field. Fill in the form and reload to see the effect. 
```
<form action="/action_page.php" autocomplete="on">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" autocomplete="off"><br><br>
  <input type="submit" value="Submit">
</form>
```

* Use maxlength for no of characters: ```maxlength="40"``` 
And use max for numeric value, use max: ```max=40```

<kbd>return</kbd>[Back to table of contents](#homepage)


----------


## HTML Input Form Attributes

HTML Input form* Attributes

The form attribute: The input form attribute Specifies the form <input> element element belongs to. It's value must be equal to the id attribute of the <form> element it belongs to. 

```
<p>The form attribute specifies the form an input element belongs to.</p>

<form action="/action_page.php" id="form1">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit">
</form>
```
```
<p>The "Last name" field below is outside the form element, but still part of the form.</p>

<label for="lname">Last name:</label>
<input type="text" id="lname" name="lname" form="form1">
```

* The formaction Attribute
The input to formaction attribute specifies the URL of the file that will process the input when the form is submitted. 

Note: This attribute overrides the action attribute of the ```<form>``` element.

The formaction attribute works with the following input types: submit and image.

```
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formaction="/action_page2.php" value="Submit as Admin">
</form>
```

* The forenctype Attribute
The input formenctype attribute specifies how the form-data should be encoded when submitted (only for forms with method="post").

Note: This attribute overrides the enctype attribute of the ```<form>``` element.

The formenctype attribute works with the following input types: submit and image.
```
<form action="/action_page_binary.asp" method="post">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formenctype="multipart/form-data" value="Submit as Multipart/form-data">
</form>
```

* The formmethod Attribute

The input formmethod attribute defines the HTTP method for sending form-data to the action URL.

Note: This attribute overrides the method attribute of the ```<form>``` element.

The formmethod attribute works with the following input types: submit and image.

The form-data can be sent as URL variables (method="get") or as an HTTP post transaction (method="post").

Notes on the "get" method:

    This method appends the form-data to the URL in name/value pairs
    This method is useful for form submissions where a user want to bookmark the result
    There is a limit to how much data you can place in a URL (varies between browsers), therefore, you cannot be sure that all of the form-data will be correctly transferred
    Never use the "get" method to pass sensitive information! (password or other sensitive information will be visible in the browser's address bar)

Notes on the "post" method:

    This method sends the form-data as an HTTP post transaction
    Form submissions with the "post" method cannot be bookmarked
    The "post" method is more robust and secure than "get", and "post" does not have size limitations

```
<form action="/action_page.php" method="get" target="_blank">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit using GET">
  <input type="submit" formmethod="post" value="Submit using POST">
</form>
```

* The formtarget Attribute

The input formtarget attribute specifies a name or a keyword that indicates where to display the response that is received after submitting the form.

Note: This attribute overrides the target attribute of the ```<form>``` element.

The formtarget attribute works with the following input types: submit and image.
```
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formtarget="_blank" value="Submit to a new window/tab">
</form>
```

* The formnovalidate Attribute
The input formnovalidate attribute specifies that an <input> element should not be validated when submitted.

Note: This attribute overrides the novalidate attribute of the ```<form>``` element.

The formnovalidate attribute works with the following input types: submit.

```
<form action="/action_page.php">
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email" required><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formnovalidate="formnovalidate" value="Submit without validation">
</form>
```

* The novalidate attribute
The novalidate attribute is a <form> attribute.

When present, novalidate specifies that all of the form-data should not be validated when submitted.
```
<form action="/action_page.php" novalidate>
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email" required><br><br>
  <input type="submit" value="Submit">
</form>
```

Chapter summary
HTML Form and Input Elements
Tag 	Description
<form> 	Defines an HTML form for user input
<input> 	Defines an input control

<kbd>return</kbd>[Back to table of contents](#homepage)



----------

## CSS Forms

CSS can enhance the looks of an HTML form. 


<!DOCTYPE html>
<html>
<style>
input[type=text], select {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
}

input[type=submit] {
  width: 100%;
  background-color: #4CAF50;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type=submit]:hover {
  background-color: #45a049;
}

div {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}
</style>
<body>

<h3>Using CSS to style an HTML Form</h3>

<div>
  <form action="/action_page.php">
    <label for="fname">First Name</label>
    <input type="text" id="fname" name="firstname" placeholder="Your name..">

    <label for="lname">Last Name</label>
    <input type="text" id="lname" name="lastname" placeholder="Your last name..">

    <label for="country">Country</label>
    <select id="country" name="country">
      <option value="australia">Australia</option>
      <option value="canada">Canada</option>
      <option value="usa">USA</option>
    </select>
  
    <input type="submit" value="Submit">
  </form>
</div>

</body>
</html>



Styling Input Fields

Use the width property to determine the width of the input field:


<!DOCTYPE html>
<html>
<head>
<style> 
input {
  width: 100%;
}
</style>
</head>
<body>

<h2>A full-width input field</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
</form>

</body>
</html>


The example above applies to all <input> elements. If you only want to style a specific input type, you can 

use attribute selectors:

    input[type=text] - will only select text fields
    input[type=password] - will only select password fields
    input[type=number] - will only select number fields
    etc..


Padded Inputs

Use the padding property to add space inside the text field.

Tip: When you have many inputs after each other, you might also want to add some margin, to add more space 

outside of them:

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
}
</style>
</head>
<body>

<h2>Padded input fields</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname">
</form>

</body>
</html>



Note that we have set the box-sizing property to border-box. This makes sure that the padding and eventually 

borders are included in the total width and height of the elements. 


Bordered Inputs

Use the border property to change the border size and color, and use the border-radius property to add 

rounded corners:

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 2px solid red;
  border-radius: 4px;
}
</style>
</head>
<body>

<h2>Input fields with borders</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname">
</form>

</body>
</html>


use border-bottom property is you only want a bottom border, as shown below:

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: none;
  border-bottom: 2px solid red;
}
</style>
</head>
<body>

<h2>Input fields with bottom border</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname">
</form>

</body>
</html>




Colored Inputs

Use the background-color property to add a background color to the input, and the color property to change 

the text color: 

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: none;
  background-color: #3CBC8D;
  color: white;
}
</style>
</head>
<body>

<h2>Input fields with color</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname" value="John">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname" value="Doe">
</form>

</body>
</html>




Focused Inputs

By default, some browsers will add a blue outline around the input when it gets focus (clicked on). You can 

remove this behavior by adding outline: none; to the input.

Use the :focus selector to do something with the input field when it gets focus:


<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 1px solid #555;
  outline: none;
}

input[type=text]:focus {
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>Input fields with color on :focus</h2>

<p>Here, the input field gets a color when it gets focus (clicked on):</p>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname" value="John">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname" value="Doe">
</form>

</body>
</html>



To change to a lightblue line during focus:


<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 3px solid #ccc;
  -webkit-transition: 0.5s;
  transition: 0.5s;
  outline: none;
}

input[type=text]:focus {
  border: 3px solid #555;
}
</style>
</head>
<body>

<h2>Input fields with black border on :focus</h2>

<p>Here, the input field gets a black border color when it gets focus (clicked on). We have also added the 

CSS transition property to animate the border color (takes 0.5 seconds to change the color on focus):</p>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname" value="John">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname" value="Doe">
</form>

</body>
</html>



Input with icon/image

If you want an icon inside the input, use the background-image property and position it with the 

background-position property. Also notice that we add a large left padding to reserve the space of the icon:

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  box-sizing: border-box;
  border: 2px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
  background-color: white;
  background-image: url('searchicon.png');
  background-position: 10px 10px; 
  background-repeat: no-repeat;
  padding: 12px 20px 12px 40px;
}
</style>
</head>
<body>

<h2>Input field with an icon inside</h2>

<form>
  <input type="text" name="search" placeholder="Search..">
</form>

</body>
</html>



Animated Search Input

In this example we use the CSS transition property to animate the width of the search input when it gets 

focus. You will learn more about the transition property later, in our CSS Transitions chapter.

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 130px;
  box-sizing: border-box;
  border: 2px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
  background-color: white;
  background-image: url('searchicon.png');
  background-position: 10px 10px; 
  background-repeat: no-repeat;
  padding: 12px 20px 12px 40px;
  transition: width 0.4s ease-in-out;
}

input[type=text]:focus {
  width: 100%;
}
</style>
</head>
<body>

<h2>Animate width of search input</h2>

<form>
  <input type="text" name="search" placeholder="Search..">
</form>

</body>
</html>



Styling Textareas

Tip: Use the resize property to prevent textareas from being resized (disable the "grabber" in the bottom 

right corner):

<!DOCTYPE html>
<html>
<head>
<style> 
textarea {
  width: 100%;
  height: 150px;
  padding: 12px 20px;
  box-sizing: border-box;
  border: 2px solid #ccc;
  border-radius: 4px;
  background-color: #f8f8f8;
  font-size: 16px;
  resize: none;
}
</style>
</head>
<body>

<h2>Styling textarea</h2>

<p><strong>Tip:</strong> Use the resize property to prevent textareas from being resized (disable the 

"grabber" in the bottom right corner):</p>

<form>
  <textarea>Some text...</textarea>
</form>

</body>
</html>




Styling Select Menus

See illustration below:


<!DOCTYPE html>
<html>
<head>
<style> 
select {
  width: 100%;
  padding: 16px 20px;
  border: none;
  border-radius: 4px;
  background-color: #f1f1f1;
}
</style>
</head>
<body>

<h2>Styling a select menu</h2>

<form>
  <select id="country" name="country">
  <option value="au">Australia</option>
  <option value="ca">Canada</option>
  <option value="usa">USA</option>
  </select>
</form>

</body>
</html>



Styling Input Buttons

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=button], input[type=submit], input[type=reset] {
  background-color: #4CAF50;
  border: none;
  color: white;
  padding: 16px 32px;
  text-decoration: none;
  margin: 4px 2px;
  cursor: pointer;
}
</style>
</head>
<body>

<h2>Styling form buttons</h2>

<input type="button" value="Button">
<input type="reset" value="Reset">
<input type="submit" value="Submit">

</body>
</html>


See CSS Buttons tutorial here: https://www.w3schools.com/css/css3_buttons.asp

Responsive Form

Resize the browser window to see the effect. When the screen is less than 600px wide, make the two columns 

stack on top of each other instead of next to each other.

Advanced: The following example use media queries to create a responsive form. You will learn more about 

this in a later chapter.



<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  resize: vertical;
}

label {
  padding: 12px 12px 12px 0;
  display: inline-block;
}

input[type=submit] {
  background-color: #4CAF50;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  float: right;
}

input[type=submit]:hover {
  background-color: #45a049;
}

.container {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}

.col-25 {
  float: left;
  width: 25%;
  margin-top: 6px;
}

.col-75 {
  float: left;
  width: 75%;
  margin-top: 6px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each 

other instead of next to each other */
@media screen and (max-width: 600px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 0;
  }
}
</style>
</head>
<body>

<h2>Responsive Form</h2>
<p>Resize the browser window to see the effect. When the screen is less than 600px wide, make the two 

columns stack on top of each other instead of next to each other.</p>

<div class="container">
  <form action="/action_page.php">
  <div class="row">
    <div class="col-25">
      <label for="fname">First Name</label>
    </div>
    <div class="col-75">
      <input type="text" id="fname" name="firstname" placeholder="Your name..">
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="lname">Last Name</label>
    </div>
    <div class="col-75">
      <input type="text" id="lname" name="lastname" placeholder="Your last name..">
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="country">Country</label>
    </div>
    <div class="col-75">
      <select id="country" name="country">
        <option value="australia">Australia</option>
        <option value="canada">Canada</option>
        <option value="usa">USA</option>
      </select>
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="subject">Subject</label>
    </div>
    <div class="col-75">
      <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>
    </div>
  </div>
  <br>
  <div class="row">
    <input type="submit" value="Submit">
  </div>
  </form>
</div>

</body>
</html>


<kbd>return</kbd>[Back to table of contents](#homepage)