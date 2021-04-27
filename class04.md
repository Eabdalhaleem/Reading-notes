# Links
 are the defining feature of the web 
because they allow you to move from 
one web page to another — enabling the 
very idea of browsing or surfing
Links are created using the *<a> element*. Users can click on anything 
between the opening <a> tag and the closing </a> tag. You specify 
which page you want to link to using the href attribute.
![aelement](https://dirask.com/static/bucket/1573242150028-jdlQB5OAR9--image.png)

------------
## Linking to Other Sites
<a>Links are created using the <a>
element which has an attribute 
called href. The value of the 
href attribute is the page that 
you want people to go to when 
they click on the link.
Users can click on anything that 
appears between the opening 
<a> tag and the closing </a>
tag and will be taken to the page 
specified in the href attribute.

-----------------

## Linking to Other Pages 
on the Same Site
When you are linking to other 
pages within the same site, 
you do not need to specify the 
domain name in the URL. You 
can use a shorthand known as a 
relative URL.
If all the pages of the site are in 
the same folder, then the value 
of the href attribute is just the 
name of the file.
If you have different pages of a 
site in different folders, then you 
can use a slightly more complex 
syntax to indicate where the 
page is in relation to the current 
page. 

---------
## Email Links
mailto:To create a link that starts up 
the user's email program and 
addresses an email to a specified 
email address, you use the <a>
element. However, this time the 
value of the href attribute starts 
with mailto: and is followed by 
the email address you want the 
email to be sent to.

-----
## Opening Links in
a New Window
target
If you want a link to open in a 
new window, you can use the 
target attribute on the opening 
<a> tag. The value of this 
attribute should be _blank.
One of the most common 
reasons a web page author 
might want a link to be opened 
in a new window is if it points to 
another website. In such cases, 
they hope the user will return 
to the window containing their 
site after finishing looking at the 
other one.

---------
## Linking to a Specific 
Part of the Same Page
Before you can link to a specific 
part of a page, you need to 
identify the points in the page 
that the link will go to. You do 
this using the id attribute (which 
can be used on every HTML 
element). You can see that the 
<h1> and <h2> elements in this 
example have been given id
attributes that identify those 
sections of the page.
The value of the id attribute 
should start with a letter or an 
underscore (not a number or 
any other character) and, on a 
single page, no two id attributes 
should have the same value.
# Linking to a Specific 
Part of Another Page
Links are created using the <a> element.
X The <a> element uses the href attribute to indicate 
the page you are linking to.
X If you are linking to a page within your own site, it is 
best to use relative links rather than qualified URLs.
X You can create links to open email programs with an 
email address in the "to" field.
X You can use the id attribute to target elements within 
a page that can be linked to.

-------
## Building Blocks
CSS treats each HTML element as if it is in its 
own box. This box will either be a block-level
box or an inline box.
Block-level boxes start on a new line and act as the main building blocks 
of any layout, while inline boxes flow between surrounding text. You can 
control how much space each box takes up by setting the width of the 
boxes (and sometimes the height, too). To separate boxes, you can use 
borders, margins, padding, and background colors

**Block-level elements**
start on a new line
Examples include:
<h1> <p> <ul> <li>

**Inline elements**
flow in between 
surrounding text
Examples include:
<img> <b> <i>

-----
## Controlling the Position of Elements
CSS has the following positioning schemes that allow you to control 
the layout of a page: normal flow, relative positioning, and absolute 
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.
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
down the page

------
##  Normal flow
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

## Relative positioning
 moves an element in relation to where it 
would have been in normal flow.
For example, you can move it 10 
pixels lower than it would have 
been in normal flow or 20% to 
the right

## When the position property 
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

## Fixed positioning 
is a type of absolute positioning that 
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
offset properties are used.

------

# WHAT IS A FUNCTION? 
Functions let you group a series of statements together to perform a 
specific task. If different parts of a script repeat the same task, you can 
reuse the function (rather than repeating the same set of statements). 

---
## Declaring Function:
to creat a function,you give it a name and then writs the statements
needed to achieve its task inside the curly braces.
this is known as a function declaration.
## Calling a function
to run the code in the function, you use the function name followed by parentheses. *sayHello();*

----
## Why pair program?
While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful

Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

* Greater efficiency
* Engaged collaboration
* Learning from fellow students
* Social skills
* Job interview readiness
* Work environment readiness
---