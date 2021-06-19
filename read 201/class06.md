# STATEMENTS 
A script is a series of instructions that a computer can follow one-by-one. 
Each individual instruction or step is known as a statement. 
Statements should end with a semicolon.

## STATEMENTS ARE INSTRUCTIONS AND EACH ONE STARTS ON A NEW LINE 
A statement is an individual instruction that the 
computer should follow. Each one should start on a 
new line and end with a semicolon. This makes your 
code easier to read and follow. 
The semicolon also tells the JavaScript interpreter 
when a step is over, indicating that it should move 
to the next step. 

----
## STATEMENTS CAN BE ORGANIZED INTO CODE BLOCKS 
Some statements are surrounded by curly braces; 
these are known as code blocks. The closing curly 
brace is not followed by a semicolon. 
Above, each code block contains one statement 
related to what the current time is. Code blocks 
will often be used to group together many more 
statements. This helps programmers organize their 
code and makes it more readable.

--------

 ## COMMENTS 
You should write comments to explain what your code does. 
They help make your code easier to read and understand. 
This can help you and others who read your code. 
/* Th i s script displays a greeting to the user based upon the current time. 
It is an example from JavaScript & jQuer y book */

----
## WHAT IS A VARIABLE?
A script will have to temporarily 
store the bits of information it 
needs to do its job. It can store this 
data in variables. 
When you write JavaScript, you have to tell the 
interpreter every individual step that you want it to 
perform. This sometimes involves more detail than 
you might expect. 
Think about calculating the area of a wall; in math 
the area of a rectangle is obtained by multiplying two 
numbers: 
width x height = are 

* A variable is a good name for this 
concept because the data stored 
in a variable can change (or vary) 
each time a script runs.

-------

# Variables: how to declare them
 in order to use the variable, you must give it a name .
 (this is sometimes called an identifier.) if a variable name is more than one word , it is usually written in **camleCase** , this  means the first word is all lower case and any subsequent words have their first letter capitlized.

![var](https://1.bp.blogspot.com/-8UmWFTngfwY/XkVRuoPFfkI/AAAAAAAACmI/93j-FMkA9EYyoRIT1qlJ2sMUbobnWT1UgCLcBGAsYHQ/s1600/javascript_var.png)


* you can now use the variable by its name, a variable's name should describe the kind of data the variable holds.
the equals sign (=)is an assignment operator .
it says that you are goingto assign a value to the variable.
is is also used to update the value given to a variable.

------
# WHAT IS AN OBJECT?
Objects group together a set of variables and functions to create a model 
of a something you would recognize from the real world. In an object, variables and functions take on new names. 

# IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES 
If a variable is part of an object, it is called a 
property. Properties tell us about the object, such as 
the name of a hotel or the number of rooms it has. 
Each individual hotel might have a different name 
and a different number of rooms.

# IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS 
If a function is part of an object, it is called a method. 
Methods represent tasks that are associated with 
the object. For example, you can check how many 
rooms are available by subtracting the number of 
booked rooms from the total number of rooms.

# Accessing an object and dot notation
you access the properties or methodes of an object using dot notation.you can also access properties using square brackets.
to  access the properties or methodes of an object you  use the name of the property you want to access.

![object](https://cdn-images-1.medium.com/max/1200/1*rSHmnlUotrjc5lXV1xDtGA.png)

-------

# The Document Object Model (DOM) specifies 
how browsers should create a model of an HTML 
page and how JavaScript can access and update the 
contents of a web page while it is in the browser window. 
The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. 
It is implemented by all major browser makers, and covers two primary areas:

## MAKING A MODEL OF THE HTM L PAGE 
When the browser loads a web page, it 
creates a model of the page in memory. 
The DOM specifies the way in which the 
browser should structure this model using 
a DOM tree. 
The DOM is called an object model 
because the model (the DOM tree) is 
made of objects. 
Each object represents a different part of 
the page loaded in the browser window.

# ACCESSING AND CHANGING THE HTML PAGE 

The DOM also defines methods and 
properties to access and update each 
object in this model, which in turn updates 
what the user sees in the browser. 
You will hear people call the DOM an 
Application Programming Interface (API). 
User interfaces let humans interact with 
programs; APls let programs (and scripts) 
talk to each other. The DOM states what 
your script can "ask the browser about the 
current page, and how to tell the browser 
to update what is being shown to the user. 


---------

# THE DOM TREE IS A 
MODEL OF A WEB PAGE 
As a browser loads a web page, it creates a model of that page. 
The model is called a DOM tree, and it is stored in the browsers' memory.It consists of four main types of nodes. 
- THE DOCUMENT NODE 
- ELEMENT NODES 
- ATTRIBUTE NODES 
- TEXT NODES 

Each node is an object with methods and properties. 
Scripts access and update this DOM tree (not the source HTML file). 
Any changes made to the DOM tree are reflected in the browser. 

![nodes](https://www.gatevidyalay.com/wp-content/uploads/2018/07/Leaf-Node-Tree-Terminology.png)

------
## WORKING WITH THE DOM TREE
Accessing and updating the DOM tree involves two steps: 
* Locate the node that represents the element you want to work with. 
* Use its text content, child elements, and attributes. 

------

The terms elements and element nodes are used interchangeably 
but when people say the DOM is working with an element, 
it is actually working with a node that represents that element. 

------
# caching Dom Queries 
methods that find elements in the DOM tree are called dom queries. when you need to work with an element mor than once , you sould use a variable to  store the result of this query.


![DOM](http://www.w3big.com/images/pic_htmltree.gif)

----
when people talk abot  storing elements in variable , they are really storing the location of the element within the DOM tree in a variable .

----
## ACCESSING ELEMENTS
DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes. 
Sometimes you will just want to access one 
individual element (or a fragment of the page that 
is stored within that one element). Other times you 
may want to select a group of element s, for example, 
every <hl> element in the page or every <1 i> 
element within a particular list. 

-----

# METHODS THAT RETURN A SINGLE ELEMENT NODE: 

**getElementByld('id')**
Selects an individual element given the value of its i d attribute . The HTML must have an id attribute in order for it to be selectable. 

**querySel ector( 'css selector')** 

Uses CSS selector syntax that would select one or more elements . This method returns only the first of the matching elements

--------------

# METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST):

**getEl ementsByClassName( 'class ' )** 
Selects one or more elements given the value of their cl ass attribute. The HTML must have a cl ass attribute for it to be selectable. This method is faster than querySe 1ectorA11 () .

**getEl ementsByTagName( 'tagName ')**
Selects all elements on the page with the specified tag name. This method is faster than querySe 1ectorA11 ().

**querySelectorAll ( 'css select or')** 
Uses CSS selector syntax to select one or more elements and returns all of those that match.

----
# getElementById() and querySelector() 
can both search  an entire document and return individual elements,both use a similar syntax. 

**getElementById()** 
is the quickest and most efficient way to access an element because no tow elements can share the same value for their id atrribute .
get El ementByi d () allows you 
to select a single element node 
by specifying the value of its 
id attribute. 
This method has one parameter: 
the value of the id attribute on 
the element you want to select. 
This value is placed inside quote 
marks because it is a string. The 
quotes can be single or double 
quotes, but they must match.

**querySelector()**
is a more recent addition to the DOM, so it is not supported in older browsers.
but its very flexibale because its parameter is a CSS selector ,which means it can be uesd to accurately target many more elements.

-----

## Selecting an element from a nodelist 
There are two ways to select an element from a Nodelist: 
The item() method and array syntax. 
Both require the index number of the element you want. 
THE ;tern{) METHOD Nodelists have a method 
called item() which will return an individual node from the 
Node list. You specify the index number of the element you want as a 
parameter of the method (inside the parentheses).
**var elements = document.getElementsByClassName('hot')** 
**if (elements.length>= 1) {** 
**var firstltem = elements.item(O);}**

--------

# ARRAY syntax 
is prefferred over the item()methode because it is faster. before selecting a node from a Nodelist , check  that it contains nodes.
if you repeatedly use the Nodelist , store it in a variable 

-------

## SELECTI NG ELEMENTS USING CLASS ATTRIBUTES 
The get El ementsByCl ass Name() method allows you to select elements whose c 1 ass attribute 
contains a specific value. The method has one parameter: 
the class name which is given in quotes within the parentheses after the method name. 
Because several elements can have the same value for their 
cl ass attribute, this method always returns a Nodelist.

## SELECTING ELEMENTS BY TAG NAME 
The get El ementsByTagName () 
method allows you to select 
elements using their tag name.  
The element name is specified 
as a parameter, so it is placed 
inside the parentheses and is 
contained by quote marks. 
Note that you do not include the 
angled brackets that surround 
the tag name in the HTML (just 
the letters inside the brackets)

## SELECTING ELEMENTS USING CSS SELECTORS 
querySe 1 ector() returns 
the first element node that 
matches the CSS-style selector. 
querySe 1ectorA11 () returns a 
Nodelist of all of the matches.Both methods take a CSS 
selector as their only parameter. 
The CSS selector syntax offers 
more flexibility and accuracy 
when selecting an element than just specifying a class name 
or a tag name, and should also 
be familiar to front-end web 
developers who are used to 
targeting elements using CSS.

---------

# Repeating actions for an entire 
when you have a Nodelist , you can loop through each node in the collection and apply the same statment to each.

-----
## TRAVERSING THE DOM 
When you have an element node, you can select 
another element in relation to it using these five 
properties. This is known as traversing the DOM. 

-------
## WHITESPACE NODES 
Traversing the DOM can be difficult because 
some browsers add a text node whenever they 
come across whitespace between elements.
Most browsers, except IE, treat 
whitespace between elements 
(such as spaces or carriage 
returns) as a text node, so the 
properties below return different 
elements in different browsers: 
previousSibling 
nextSiblfng 
firstChild 
lastChild 

-----

## PREVIOUS & NEXT SIBLING 
You have just seen that 
these properties can return 
inconsistent results in different 
browsers. However, it is safe 
to use them when there is no 
whitespace between elements. 
For this example, all spaces 
between the HTML elements 
have been removed. In order to 
demonstrate these properties, 
the second list item is selected 
using getEl ementByld (). 
From this element node, the 
previ ousSi b 1 i ng property will 
return the first <1 i> element, 
and the next Sib 1 i ng property 
will return the third <1 i> 
element. 

---------

**FlRST & LAST CHILD**
These properties also return 
inconsistent results if there is 
whitespace between elements. 
In this example, a slightly 
different solution is used in the 
HTML - the closing tags are put 

next to the opening tags of 
the next element, making it 
a little more readable. The 
example starts by using the 
getElementsByTagName() 
method to select the <ul>
element from the page. From this 
element node, the fi rstChi 1 d 
property will return the first <1 i > 
element, and the 1 as tChi 1 d 
property will return the last <l i > 
element.

-------

## HOW TO GET/UPDATE ELEMENT CONTENT 
So far this chapter has focused on finding elements in the DOM tree. 
The rest of this chapter shows how to access/update element content. 
Your choice of techniques depends upon what the element contains. 

*ACCESS & UPDATE A TEXT NODE WITH NODEVALUE* 
When you select a text node, you can retrieve or amend the content of it 
using the node Va 1 ue property.

--------

## Adding  or removing  HTML content:
there are two very different  approaches to adding and removing content from a DOM tree : the **innerHTML** property and DOM manipulation.

## DOM manipulation 
easliy targets individual nodes in th DOM tree , whereas **innerHTML** is better suited to updating entire fragments.

-------

## Attribute Nodes 
once you have an element node , you can use other properties and methodes on that element node to  access and change its attributes.

## CHECK FOR AN ATTRIBUTE AND GET ITS VALUES 
Before you work with an 
attribute, it is good practice to 
check whether it exists. This will 
save resources if the attribute 
cannot be found.The hasAttri bute() method 
of any element node lets you 
check if an attribute exists. The 
attribute name is given as an 
argument in the parentheses. Using hasAttribute() in an if 
statement like this means that 
the code inside the curly braces 
will run only if the attribute 
exists on the given element. 

----------

## CREATING ATTRIBUTES & CHANGING THEIR VALUES 
The className property allows 
you to change the value of the 
class attribute. If the attribute 
does not exist, it will be created 
and given the specified value. You have seen this property 
used throughout the chapter 
to update the status of the 
list items. Below, you can see 
another way to achieve the task. 
The setAttri bute() method 
allows you to update the value 
of any attribute. It takes two 
parameters: the attribute name, 
and the value for the attribute. 

---------
## REMOVING ATTRI BUTES
To remove an attribute from an 
element, first select the element, 
then call removeAtt r i bute () . 
It has one parameter: the name 
of the attribute to remove.  
Trying to remove an attribute 
that does not exist will not cause 
an error, but it is good practice 
to check for its existence before 
attempting to remove it

-------

- The browser represents the page using a DOM tree. 
- DOM trees have four types of nodes: document nodes,
 
 element nodes, attribute nodes, and text nodes. 
- You can select element nodes by their id or class  
 attributes, by tag name, or using CSS selector syntax. 

- Whenever a DOM query can return more than one 
 node, it will always return a Nadelist.

- From an element node, you can access and update its 
 content using properties such as textContent and 
 innerHTML or using DOM manipulation techniques.

- An element node can contain multiple text nodes and 
 child elements that are siblings of each other.
  
- In older browsers, implementation of the DOM is 
 inconsistent (and is a popular reason for using jQuery). 
 Browsers offer tools for viewing the DOM tree . 


 
