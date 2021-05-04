# layout 

Key Concepts in Positioning Elements

Building Blocks.

CSS treats each HTML element as if it is in its 
own box.This box will either be a block-level
box or an inline box.

Block-level boxes start on a new line and act as the main building blocks 
of any layout, while inline boxes flow between surrounding text. You can 
control how much space each box takes up by setting the width of the 
boxes (and sometimes the height, too). To separate boxes, you can use 
borders, margins, padding, and background colors.

-----------

Block-level elementsstart on a new line
Examples include:
<h1> <p> <ul> <li>


Inline elementsflow in between surrounding text
Examples include:
<img> <b> <i>

-------------

# Containing Elements

If one block-level element sits inside another 
block-level element then the outer box is 
known as the containing or parent element.

It is common to group a number of elements together inside a <div>

(or other block-level) element. For example, you might group together 
all of the elements that form the header of a site (such as the logo and 
the main navigation). The <div> element that contains this group of 
elements is then referred to as the containing element

-----------

## Controlling the Position of Elements

CSS has the following positioning schemes that allow you to control 
the layout of a page: normal flow, relative positioning, and absolute 
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.

-------

**Normal flow**

Every block-level element 
appears on a new line, causing 
each item to appear lower down 
the page than the previous one. 
Even if you specify the width 
of the boxes and there is space 
for two elements to sit side-byside, they will not appear next 
to each other. This is the default 
behavior (unless you tell the 
browser to do something else).

---

**Relative Positioning**

This moves an element from the 
position it would be in normal 
flow, shifting it to the top, right, 
bottom, or left of where it 
would have been placed. This 
does not affect the position of 
surrounding elements; they stay 
in the position they would be in 
in normal flow

-----

**Absolute positioning**

This positions the element 
in relation to its containing 
element. It is taken out of 
normal flow, meaning that it 
does not affect the position 
of any surrounding elements 
(as they simply ignore the 
space it would have taken up). 
Absolutely positioned elements 
move as users scroll up and 
down the page.

--------

To indicate where a box should be positioned, you may also need to use 
box offset properties to tell the browser how far from the top or bottom 
and left or right it should be placed

------

**Fixed Positioning**

This is a form of absolute 
positioning that positions 
the element in relation to the 
browser window, as opposed 
to the containing element. 
Elements with fixed positioning 
do not affect the position of 
surrounding elements and they 
do not move when the user 
scrolls up or down the page.

----

**Floating Elements**

Floating an element allows 
you to take that element out 
of normal flow and position 
it to the far left or right of a 
containing box. The floated 
element becomes a block-level 
element around which other 
content can flow.

------

## Normal Flow
 **position:static**

 In normal flow, each block-level 
element sits on top of the next 
one. Since this is the default 
way in which browsers treat 
HTML elements, you do not 
need a CSS property to indicate 
that elements should appear 
in normal flow, but the syntax 
would be:
position: static; 
I have not specified a width
property for the heading 
element, so you can see how it 
stretches the width of the entire 
browser window by default.
The paragraphs are restricted 
to 450 pixels wide. This shows 
how the elements in normal flow 
start on a new line even if they 
do not take up the full width of 
the browser window.

----------

# Relative Positioning

**position:relative**

Relative positioning moves an 
element in relation to where it 
would have been in normal flow.
For example, you can move it 10 
pixels lower than it would have 
been in normal flow or 20% to 
the right.
You can indicate that an element 
should be relatively positioned 
using the position property 
with a value of relative.

------

# Absolute Positioning

**position:absolute**

When the position property 
is given a value of absolute, 
the box is taken out of normal 
flow and no longer affects the 
position of other elements on 
the page. (They act like it is not 
there.) 
The box offset properties (top
or bottom and left or right) 
specify where the element 
should appear in relation to its 
containing element

-------

# Fixed Positioning

**position:fixed**

Fixed positioning is a type 
of absolute positioning that 
requires the position property 
to have a value of fixed.
It positions the element in 
relation to the browser window. 
Therefore, when a user scrolls 
down the page, it stays in the 
exact same place. It is a good 
idea to try this example in your 
browser to see the effect.
To control where the fixed 
position box appears in relation 
to the browser window, the box 
offset properties are used

--------

# Overlapping Elements

**z-index**

When you use relative, fixed, or 
absolute positioning, boxes can 
overlap. If boxes do overlap, the 
elements that appear later in the 
HTML code sit on top of those 
that are earlier in the page. 
If you want to control which 
element sits on top, you can use 
the z-index property. Its value 
is a number, and the higher the 
number the closer that element 
is to the front

----------

# Floating Elements
 
 **float**

 The float property allows you 
to take an element in normal 
flow and place it as far to the 
left or right of the containing 
element as possible.
Anything else that sits inside 
the containing element will 
flow around the element that is 
floated.
When you use the float
property, you should also use the 
width property to indicate how 
wide the floated element should 
be. If you do not, results can be 
inconsistent but the box is likely 
to take up the full width of the 
containing element (just like it 
would in normal flow).

---------
# Using Float to Place Elements Side-by-Side

A lot of layouts place boxes 
next to each other. The float
property is commonly used to 
achieve this.
When elements are floated, the 
height of the boxes can affect 
where the following elements sit.
In this example, you can see six 
paragraphs, each of which has a 
width and a float property set.

---------

# Clearing Floats
 
 ## clear

 The clear property allows you 
to say that no element (within 
the same containing element) 
should touch the left or righthand sides of a box. It can take 
the following value

**left**

The left-hand side of the box 
should not touch any other 
elements appearing in the same 
containing element.

**right**

The right-hand side of the 
box will not touch elements 
appearing in the same containing 
element.


**both**

Neither the left nor right-hand 
sides of the box will touch 
elements appearing in the same 
containing element.


**none**

Elements can touch either side.
In this example, the fourth 
paragraph has a class called 
clear. The CSS rule for this 
class uses the clear property 
to indicate that nothing should 
touch the left-hand side of it. The 
fourth paragraph is therefore 
moved further down the page 
so no other element touches its 
left-hand side

----------

## Parents of Floated Elements: Problem

If a containing element only
contains floated elements, some 
browsers will treat it as if it is 
zero pixels tall.
As you can see in this example, 
the one pixel border assigned 
to the containing element has 
collapsed, so the box looks like a 
two pixel line

-------

# Parents of Floated Elements: Solution

raditionally, developers got 
around this problem by adding 
an extra element after the 
last floated box (inside the 
containing element).

A CSS rule would be applied to this 
additional element setting the 
clear property to have a value 
of both. But this meant that an 
extra element was added to the 
HTML just to fix the height of the 
containing element.

More recently, developers have 
opted for a purely CSS-based 
solution because it means that 
there is no need to add an extra 
element to the HTML page after 
the floated elements.
 The pure CSS solution adds two CSS rules 
to the containing element .

----------

## Creating Multi-Column Layouts with Floats

Many web pages use multiple 
columns in their design. This 
is achieved by using a <div>
element to represent each 
column. The following three CSS 
properties are used to position 
the columns next to each other: 

**width**
This sets the width of the 
columns.

**float**
This positions the columns next 
to each other.

**margin**
This creates a gap between the 
columns.

---------

# screen Sizes

Different visitors to your site will have different sized screens that show 
different amounts of information, so your design needs to be able to 
work on a range of different sized screens.

---------

# Screen Resolution

Resolution refers to the number of dots a screen shows per inch. Some 
devices have a higher resolution than desktop computers and most 
operating systems allow users to adjust the resolution of their screens.

---------

# Page Sizes

Because screen sizes and display resolutions vary so much, web 
designers often try to create pages of around 960-1000 pixels wide 
(since most users will be able to see designs this wide on their screens).

-------------

# Fixed Width Layouts

Fixed width layout designs do not 
change size as the user increases 
or decreases the size of their 
browser window. Measurements tend 
to be given in pixels.

## Advantages

* Pixel values are accurate 
at controlling size and 
positioning of elements.

* The designer has far greater 
control over the appearance 
and position of items on the 
page than with liquid layouts.

* You can control the lengths 
of lines of text regardless of 
the size of the user's window.

* The size of an image will 
always remain the same 
relative to the rest of the 
page.

----------

## Disadvantages

* You can end up with big gaps 
around the edge of a page.

* If the user's screen is a much 
higher resolution than the 
designer's screen, the page 
can look smaller and text can 
be harder to read.

* If a user increases font sizes, 
text might not fit into the 
allotted spaces.

* The design works best on 
devices that have a site or 
resolution similar to that of 
desktop or laptop computers. 

* The page will often take up 
more vertical space than a 
liquid layout with the same 
content.


---------

## Liquid Layouts

Liquid layout designs 
stretch and contract 
as the user increases 
or decreases the 
size of their browser 
window. They tend to 
use percentages

---
## A Fixed Width Layout

To create a fixed width layout, 
the width of the main boxes on 
a page will usually be specified 
in pixels (and sometimes their 
height, too).

Here you can see several <div>
elements, each of which uses an 
id or class attribute to indicate 
its purpose on the page.

In a book like this, the result of 
both the fixed and liquid layouts 
look similar. To get a real feel for 
them, you need to view them in 
your browser and see how they 
react when you adjust the size of 
the browser window.

The fixed width layout will stay 
the same width no matter what 
size the browser window is, 
whereas the liquid layout will 
stretch (or shrink) to fill the 
screen.

The HTML is the same for both 
the fixed width layout example 
on this page and the liquid layout 
example you see next.

----------

The rule for the <body> element 
is used to fix the width of the 
page at 960 pixels, and it is 
centered by setting the left and 
right margins to auto. 
The main boxes on the page 
have a margin of 10 pixels to 
create a gap between them.
The navigation, feature, and 
footer panels stretch to the 
width of the containing element 
(which in this instance is the 
<body> element), so we do not 
need to specify a width for them.
The three columns are each 300 
pixels wide and use the float
property, which allows them to 
sit next to each other

----------


# A Liquid Layout

The liquid layout uses 
percentages to specify the width 
of each box so that the design 
will stretch to fit the size of the 
screen.
When trying this in your 
browser, remember to make the 
window smaller and larger.


--------

There is a rule on the <body>
element to set the width of the 
page to 90% so that there is a 
small gap between the left and 
right-hand sides of the browser 
window and the main content.
The three columns are all given 
a margin of 1% and a width of 
31.3%. This adds up to 99.9% 
of the width of the <body>
element, so some browsers 
might not perfectly align the 
right-hand side of the third 
column with other elements on 
the page. 
The <div> elements that hold 
the navigation, feature, and 
footer will stretch to fill the 
width of the containing <body>
element. They are given a 1% 
margin to help them align with 
the columns.

![layout](https://www.htmlgoodies.com/wp-content/uploads/2021/04/Example-1.png)

-----------

# Layout Grids

Composition in any visual art (such as design, painting, or photography) 
is the placement or arrangement of visual elements — how they are 
organized on a page. Many designers use a grid structure to help them 
position items on a page, and the same is true for web designer

--------

## CSS Frameworks

CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS 
framework code in your projects rather than writing the CSS from scratch.

**ADVANTAGES**

* They save you from 
repeatedly writing code for 
the same tasks.

* They will have been tested 
across different browser 
versions (which helps avoid 
browser bugs)



 **DISADVANTAGES**
* They often require that you 
use class names in your 
HTML code that only control 
the presentation of the page 
(rather than describe its 
content)

----------

# Using the 960.GS Grid

Below you can see a sample layout of a page just like the fixed width page example. 
stylesheet. Instead of writing our own CSS to control layout, we will need 
to add classes to the HTML indicating how wide each section should be

-------

# A Grid-Based Layout 

Let's take a look at an HTML 
page and how it has been 
marked up to use the 960.gs grid 
system.

You can see that we include 
the CSS for the grid using the 
<link> element inside the 
<head> of the page.

The styles we are writing 
ourselves are shown on the right 
hand page.

The 960_12_col.css stylesheet 
contains all of the rules we need 
to control the grid layout. The 
HTML uses the class names:
container_12 to act as a 
container for the whole page and 
indicate that we are using a 12 
column grid

![layout1](https://data-flair.training/blogs/wp-content/uploads/sites/2/2020/07/HTML-Layout-df.jpg)

----------

# Multiple Style Sheets

**@import**

Some web page authors split 
up their CSS style rules into 
separate style sheets. For 
example, they might use one 
style sheet to control the layout 
and another to control fonts, 
colors and so on.

Some authors take an even 
more modular approach 
to stylesheets, creating 
separate stylesheets to control 
typography, layout, forms, 
tables, even different styles for 
each sub-section of a site

--------

# Multiple Style Sheets

**link**

On this page you can see the 
other technique for including 
multiple style sheets. Inside the 
<head> element is a separate 
<link> element for each style 
sheet.

The contents of site.css are 
identical to styles.css on the 
left hand page, except the code 
does not contain @import rules.
As with all style sheets, if two 
rules apply to the same element 
then rules that appear later in a 
document will take precedence 
over previous rules. 

----------

* <div> elements are often used as containing elements 
to group together sections of a page.

* Browsers display pages in normal flow unless you 
specify relative, absolute, or fixed positioning.

* The float property moves content to the left or right 
of the page and can be used to create multi-column 
layouts. (Floated items require a defined width.)

* Pages can be fixed width or liquid (stretchy) layouts.

* Designers keep pages within 960-1000 pixels wide, 
and indicate what the site is about within the top 600 
pixels (to demonstrate its relevance without scrolling).

* Grids help create professional and flexible designs.

* CSS Frameworks provide rules for common tasks.

* You can include multiple CSS files in one page


