
CSS Multiple Columns .edit { background-color:#f1f1f1; color:red; } .container { border:1px solid #ddd; width:100%; margin:0; } .header { background-color:#f1f1f1; text-align:center; font-size:30px; padding:40px 0; } .parent { width:100%; margin:0; } .child1, .child2, .child3 { float:left; max-width:33%; padding:10px; box-sizing:border-box; } .child1, .child2 { border-right:1px solid #ddd; } .parent::after { content:""; clear:both; display:table; } .table1 { width:100%; border:1px solid #ddd; border-collapse:collapse; } .table1 th { text-align:left; font-weight:normal; padding-left:10px; border:1px solid #ddd; } .table1 td { text-align:center; border:1px solid #ddd; } .table1 tr { height:40px; } .table1 tr:nth-child(even) { background-color:#f1f1f1; } .columncount { column-count:3; } .columngap { column-count:3; column-gap:40px; } .columnrulestyle { column-count:3; column-gap:40px; column-rule-style:solid; } .columnrulewidth { column-count:3; column-gap:40px; column-rule-style:solid; column-rule-width:1px; } .columnrulecolor { column-count:3; column-gap:40px; column-rule-style:solid; column-rule-width:1px; column-rule-color:lightblue; } .columnrule { column-count:3; column-gap:40px; column-rule:1px solid lightblue; } .columnspan { column-count:3; column-gap:40px; column-rule:1px solid lightblue; } .columnspan h2 { column-span:all; text-align:center; } .columnwidth { column-width:100px; } .table2 { width:70%; border:1px solid #f1f1f1; border-collapse:collapse; } .table2 tr { height:40px; } .table2 tr:nth-child(even) { background-color:#f1f1f1; } .table2 th { text-align:left; padding-left:10px; } .table2 td:first-child { padding-left:10px; }

CSS Multiple Columns
====================

* * *

CSS Multi-column Layout
-----------------------

The CSS multi-column layout allows easy definition of multiple columns of text - just like in newspapers.  
Example:-  

Daily Ping

Lorem ipsum
-----------

dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation

ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio

dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.

* * *

CSS Multi-column Properties
---------------------------

In this chapter you will learn about the following multi-column properties:-  

*   column-count
*   column-gap
*   column-rule-style
*   column-rule-width
*   column-rule-color
*   column-rule
*   column-span
*   column-width

* * *

Browser Support
---------------

The numbers in the table specify the first browser version that fully supports the property.  



|    Property      |  Google Chrome|  Microsoft Edge| Mozilla Firefox|  Apple Safari |     Opera     |
|-------------------|---------------|----------------|---------------|---------------|---------------|
|  column-count     |     50.0      |       10.0     |      52.0     |      9.0      |      37.0     |
|  column-gap       |     50.0      |       10.0     |      52.0     |      9.0      |      37.0     |
|  column-rule      |     50.0      |       10.0     |      52.0     |      9.0      |      37.0     |
|  column-rule-color|     50.0      |       10.0     |      52.0     |      9.0      |      37.0     |
|  column-rule-style|     50.0      |       10.0     |      52.0     |      9.0      |      37.0     |
|  column-rule-width|     50.0      |       10.0     |      52.0     |      9.0      |      37.0     |
|  column-span      |     50.0      |       10.0     |      71.0     |      9.0      |      37.0     |
|  column-width     |     50.0      |       10.0     |      52.
* * *

  
  

* * *

CSS Create Multiple Columns
---------------------------

The column-count property specifies the number of columns an element should be divided into.  
The following example will divide the text in the <div> element into 3 columns.  
Example:-  

Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.

* * *

CSS Specify the Gap Between Columns
-----------------------------------

The column-gap property specifies the gap between the columns.  
The following example specifies a 40 pixels gap between the columns.  
Example:-  

Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.

* * *

CSS Column Rules
----------------

The column-rule-style property specifies the style of the rule between columns.  
Example:-  

Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.

  
  
The column-rule-width property specifies the width of the rule between columns.  
Example:-  

Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.

  
  
The column-rule-color property specifies the color of the rule between columns.  
Example:-  

Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.

  
  
The column-rule property is a shorthand property for setting all the column-rule-\* properties above.  
The following example sets the width, style, and color of the rule between columns.  
Example:-  

Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.

* * *

Specify How Many Columns an Element Should Span
-----------------------------------------------

The column-span property specifies how many columns an element should span across.  
The following example specifies that the <h2> element should span across all columns.  
Example:-  

Lorem Ipsum Dolor Sit Amet
--------------------------

Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.

* * *

Specify The Column Width
------------------------

The column-width property specifies a suggested, optimal width for the columns.  
The following example specifies that the suggested, optimal width for the columns should be 100px.  
Example:-  

Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.

* * *

CSS Multi-columns Properties
----------------------------

The following table lists all the multi-columns properties.  

Property

Description

column-count

Specifies the number of columns an element should be divided into

column-fill

Specifies how to fill columns

column-gap

Specifies the gap between the columns

column-rule

A shorthand property for setting all the column-rule-\* properties

column-rule-color

Specifies the color of the rule between columns

column-rule-style

Specifies the style of the rule between columns

column-rule-width

Specifies the width of the rule between columns

column-span

Specifies how many columns an element should span across

column-width

Specifies a suggested, optimal width for the columns

columns

A shorthand property for setting column-width and column-count



# Local Override Global 1

<style>
:root {
  --blue: #1e90ff;
  --white: #ffffff;
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
}

button {
  --blue: #0000ff; /* local variable will override global */
  background-color: var(--white);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}
</style>

## Override Global Variable With Local Variable

Lorem Ipsum

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at pulvinar felis blandit.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at pulvinar felis blandit.

<button>Yes</button>
<button>No</button>