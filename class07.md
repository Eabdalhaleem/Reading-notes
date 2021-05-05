# Tables
## What's a Table?

A table represents information in a grid format. 
Examples of tables include financial reports, TV 
schedules, and sports results

## Basic Table Structure

`<table>`
The `<table>` element is used 
to create a table. The contents 
of the table are written out row 
by row.


![tables](http://3.bp.blogspot.com/-m3yVfQjKy50/VWr2wjykduI/AAAAAAAAO-4/DEe2-YYq6Pw/s1600/HTML-table-shortcode.jpg)


------------

`<tr>`
You indicate the start of each 
row using the opening `<tr>` tag. 
(The tr stands for table row.) 
It is followed by one or more

-----------

`<td>` elements (one for each cell 
in that row). 
At the end of the row you use a 
closing `</tr>` tag.

------------

`<td>`
Each cell of a table is 
represented using a `<td>`
element. (The td stands for 
table data.)
At the end of each cell you use a 
closing `</td>` tag

------------

## Table Headings

`<th>`
The `<th>` element is used just 
like the `<td>` element but its 
purpose is to represent the 
heading for either a column or 
a row. (The th stands for table 
heading.)

----------

# Long Tables

There are three elements that 
help distinguish between the 
main content of the table and 
the first and last rows (which can 
contain different content).
These elements help people 
who use screen readers and also 
allow you to style these sections 
in a different manner than the 
rest of the table (as you will see 
when you learn about CSS).

`<thead>`
The headings of the table should 
sit inside the `<thead>` element. 

`<tbody>`
The body should sit inside the 
`<tbody>` element.

`<tfoot>`
The footer belongs inside the 
`<tfoot>` element

---------

Old Code:
# Width & Spacing

There are some outdated 
attributes which you should not 
use on new websites. You may, 
however, come across some 
of them when looking at older 
code, so I will mention them 
here. All of these attributes have 
been replaced by the use of CSS.
The width attribute was used 
on the opening `<table>` tag to 
indicate how wide that table 
should be and on some opening 
`<th>` and `<td>` tags to specify 
the width of individual cells. 
The value of this attribute is 
the width of the table or cell in 
pixels.

The columns in a table need to 
form a straight line, so you often 
only see the width attribute on 
the first row (and all subsequent 
rows would use that setting).
The opening `<table>` tag could 
also use the cellpadding
attribute to add space inside 
each cell of the table, and the 
cellspacing attribute to create 
space between each cell of 
the table. The values for these 
attributes were given in pixels.

-----------

* The `<table>` element is used to add tables to a web 
page.

* A table is drawn out row by row. Each row is created 
with the `<tr>` element.

* Inside each row there are a number of cells 
represented by the `<td>` element (or `<th>` if it is a 
header).

* You can make cells of a table span more than one row 
or column using the rowspan and colspan attributes.

* For long tables you can split the table into a `<thead>`, 
`<tbody>`, and `<tfoot>`

-----------------


# Creatingan object :constructor notation

the new keyword and the object constructor create a blank object.

# ubdating an object
to update the value of properties , use dot notation o rsquare brackets,
they work on object created using literal or constructor notation.
to delete a property ,use thr delete keyword

----------
# creating many object: constructor notation

sometimes you will want several object to represent similar things .
object constructors can use a function as a template for creating object.
first , create the template wirh the object properties and mothods.

![object](https://res.cloudinary.com/practicaldev/image/fetch/s--rJeH0yGE--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/t52ni02srb8688lh3eh8.png)

---------------

you create instances of the object using the constuctor function.
the new keyword followed by a call tothe function creates a new objact.
the properties of each object are given as arguments to the function.

![create](https://miro.medium.com/max/795/1*rSHmnlUotrjc5lXV1xDtGA.png)

-----

## CREATING OBJECTS USING CONSTRUCTOR SYNTAX 

On the right, an empty object 
called hote 1 is created using the 
constructor function. 
Once it has been created, three 
properties and a method are 
then assigned to the object. 
(If the object already had any 
of these properties, this would 
overwrite the values in those 
properties.) 
To access a property of this 
object, you can use dot notation, 
just as you can with any object.

-----

# CREATE & ACCESS OBJECTS CONSTRUCTOR NOTATION



First, a constructor function 
defines a template for the hotels. 
Next, two different instances 
of this type of hotel object are 
created. The first represents 
a hotel called Quay and the 
second a hotel called Park.

Having created instances of 
these objects, you can then 
access their properties and 
methods using the same dot 
notation that you use with all 
other objects.

-----------

## RECAP: WAYS TO CREATE OBJECTS

* CREATE THE OBJECT, THEN ADD PROPERTIES & METHODS 
In both of these examples, the object is created on 
the first line of the code sample. The properties and 
methods are then added to it afterwards. 

Once you have created an object, the syntax for 
adding or removing any properties and methods 
from that object is the same.

* CREATING AN OBJECT WITH PROPERTIES & METHODS 
LITERAL NOTATION 
A colon separates the key/value pairs. 
There is a comma between each key/value pair. 

* OBJECT CONSTRUCTOR NOTATION 
The function can be used to create multiple objects. 
The this keyword is used instead of the object name. 

--------

# THIS (IT IS A KEYWORD)

The keyword this is commonly used inside functions and objects. 
Where the function is declared alters what this means. It always refers 
to one object, usually the object in which the function operates. 

**A FUNCTION IN GLOBAL SCOPE**

When a function is created at the top level of a script 
(that is, not inside another object or function), then it 
is in the global scope or global context.

The default object in this context is the window 
object. so when this is used inside a function in the 
global context it refers to the window object.

**GLOBAL VARIABLES**

All global variables also become properties of the 
window object. so when a function is in the global 
context, you can access global variables using the 
window object, as well as its other properties.


**A METHOD OF AN OBJECT** 

When a function is defined inside an object, it 
becomes a method. In a method, this refers to the 
containing object. 

**FUNCTION EXPRESSION AS METHOD**

If a named function has been defined in global 
scope, and it is then used as a method of an object, 
this refers to the object it is contained within.


--------

# RECAP: STORING DATA

In JavaScript, data is represented using name/value pairs. 
To organize your data, you can use an array or object to group a set of 
related values. In arrays and objects the name is also known as a key. 

---

**VARIABLES**

A variable has just one key (the variable name) 
and one value. 
Variable names are separated from their value by an 
equals sign (the assignment operator): 
*var hotel= 'Quay' ;*

--

**ARRAYS** 
Arrays can store multiple pieces of information. 
Each piece of information is separated by a comma. 
The order of the values is important because items 
in an array are assigned a number (called an index). 
Values in an array are put in square brackets, 
separated by commas:
var hotel s = [ ' Quay ' , ' Park' , ' Beach' , 'Bloomsbury' ]

------

If you want to access items via a property name or key, use an object 
(but note that each key in the object must be unique). 
If the order of the items is important, use an array. 


**INDIVIDUAL OBJECTS**

Objects store sets of name/value pairs. They can be 
properties (variables) or methods (functions). 
The order of them is not important (unlike the array). 
You access each piece of data by its key. 
In object literal notation, properties and methods of 
an object are given in curly braces: 
var hotel = {name: 'Quay', rooms: 40};

-------

**MULTIPLE OBJECTS** 

When you need to create multiple objects within the 
same page, you should use an object constructor to 
provide a template for the objects. 
function Hotel (name, rooms) 
this .name = name; 
this.rooms = rooms; 
You then create instances of the object using the new 
keyword and then a call to the constructor function. 
var hotell =new Hotel ( 'Quay', 40); 
var hotel2 = new Hotel ( ' Park ' , 120);


------

# Arrays are Object

Arrays are a ctually a special type of object.they hold a related set of key/value paris(like all object), but the key for each value is its index number.

------

# Arrays of object &objects in arrays

you can combine arrays and object to create complex data structures;arrays can store
a series of pbject (and remember their order).object can also hold arrays (as values of their pyoperties)

in an object,the order in which the properties appear is not important.in an array, the index number dictate the order of the properties.

## Arrays in an object 
the property of any object can hold any array.

## object in am array
the value of any element in an array can be an object .

----

The objects you create will usually be specifically 
written to suit your needs. They model the data 
used within, or contain functionality needed by, 
your script. Whereas, the built-in objects contain 
functionality commonly needed by many scripts. 
As soon as a web page has loaded into the browser, 
these objects are available to use in your scripts. 
 
These built-in objects help you get a wide range 
of information such as the width of the browser 
window, the content of the main heading in the page, 
or the length of text a user entered into a form field. 
You access their properties or methods using dot 
notation, just like you would access the properties or 
methods of an object you had written yourself.

--------

## three groups of built in object

* using built in object:
the three sets of built in object each offer a different range of tools that help you write scripts for web pages.

* browser object model:
the browser object model of the beowser tab or windows. the top most object is the window object,which represents current browser window or tab ,its child object represent other browser features.

--------
 
# THE BROWSER OBJECT MODEL: 
## THE WINDOW OBJECT 
The window object represents the current 
browser window or tab. It is the topmost object 
in the Browser Object Model, and it contains 
other objects that tell you about the browser. 

-----------

USING THE BROWSER 
OBJECT MODEL 
Here, data about the browser is 
collected from the window object 
and its children, stored in the msg 
variable, and shown in the page. 
The+= operator adds data onto 
the end of the msg variable.

1. Two of the window object's 
properties, i nnerWi dth and 
i nnerHei ght, show width and 
height of the browser window. 

2. Child objects are stored as 
properties of t heir parent object. 
So dot notation is used to access 
them, just like you would access 
any other property of that object. 
In turn, to access the properties 
of the child object, another dot is 
used between the child object's 
name and its properties, 
e.g., window. history . length 

3. The element whose id 
attribute has a value of info is 
selected, and the message that 
has been built up to this point is 
written into the page. 

-------------

## THE DOCUMENT OBJECT MODEL: 
**THE DOCUMENT OBJECT**
The topmost object in the Document Object Model (or DOM) is the 
document object. It represents the web page loaded into the current 
browser window or tab.

-------

## GLOBAL OBJECTS: STRING O BJECT 
Whenever you have a value that is a string, you can use the properties 
and methods of the String object on that value. This example stores the 
phrase "Home sweet home " in a variable. 

 **var saying = 'Home sweet home ;**

 -------

## DATA TYPES REVISITED 
In JavaScript there are six data types: 
Five of them are described as simple (or primitive) data types. 
The sixth is the object (and is referred to as a complex data type). 

## SIMPLE OR PRIMITIVE DATA TYPES

JavaScript has five simple (or primitive) data types: 
1. String 
2. Number 
3. Boolean 
4. Undefined (a variable that has been declared, but 
no value has been assigned to it yet) 
5. Null (a variable with no value - it may have had 
one at some point, but no longer has a value) 
As you have seen, both the web browser and the 
current document can be modeled using objects 
(and objects can have methods and properties).

But it can be confusing to discover that a simple 
value **(like a string, a number, or a Boolean)** can have 
methods and properties. Under the hood, JavaScript 
treats every variable as an object in its own right.

**String:** If a variable, or the property of an object, 
contains a string, you can use the properties and 
methods of the String object on it. 

**Number:** If a variable, or property of an object, 
stores a number, you can use the properties and 
methods of the Number object on it .

**Boolean:** There is a Boo 1 ean object. It is rarely used. 
(Undefined and null values do not have objects.) 

---

## COMPLEX DATA TYPE 
JavaScript also defines a complex data type: 
**6.0bject** 
Under the hood, arrays and functions are considered 
types of objects.

**ARRAYS ARE OBJECTS** 
As you saw on p118, an array is a set of key/value 
pairs (just like any other object). But you do not 
specify the name in the key/value pair of an array - it 
is an index number.

like other objects, arrays have properties and 
methods. On p72 you saw that arrays have a 
property called 1 ength, which tells you how many 
items are in that array. There is also a set of methods 
you can use with any array to add items to it, remove 
items from it, or reorder its contents. 

![array](https://johannafaith.com/media/javascript-array-of-objects-example.png)

-----------

**FUNCTIONS ARE OBJECTS** 

Technically, functions are also objects. But they 
have an additional feature: they are callable, which 
means you can tell the interpreter when you want to 
execute the statements that it contains.

------

**GLOBAL OBJECTS: NUMBER OBJECT** 
Whenever you have a value that is a number, 
you can use the methods and properties of the 
Number object on it.

-----

**WORKING WITH DECIMAL NUMBERS**

As with the String object the 
properties and methods of the 
Number object can be used with 
with any value that is a number

-------

**GLOBAL OBJECTS: MATH OBJECT**
The Math object has properties and methods 
for mathematical constants and functions.

![globel](https://poiemaweb.com/img/object.png)


--------

## Creating an instance of the date object 
in order to work with dates, you create an instance of the Data object.
you can then specify the time and data that you want it to represent.

* to create a Data object , use the Data () object constructor.the syntax is the same for creating any object with a constructor function.

--

* Functions allow you to group a set of related 
statements together that represent a single task. 

* Functions can take parameters (informatiorJ required 
to do their job) and may return a value.

* An object is a series of variables and functions that 
represent something from the world around you. 
* In an object, variables are known as properties of the 
object; functions are known as methods of the object.

* Web browsers implement objects that represent both 
the browser window and the document loaded into the 
browser window.

* JavaScript also has several built-in objects such as 
String, Number, Math, and Date. Their properties and 
methods offer functionality that help you write scripts.

* Arrays and objects can be used to create complex data 
sets (and both can contain the other). 

---------

**Domain Modeling**
Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

**Model epic fails videos**
Imagine you've been tasked to build a program that models the popularity of epic fail videos. After months of painstaking research, you've determined that the two essential metrics for gauging popularity are an epic rating and whether or not the video has animals.

**Define a constructor and initialize properties**
To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.

----------

* Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

Here's some tips to follow when building your own domain models.

* When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
* Model its attributes with a constructor function that defines and initializes properties.
* Model its behaviors with small methods that focus on doing one job well.
* Create instances using the new keyword followed by a call to a constructor function.
* Store the newly created object in a variable so you can access its properties and methods from outside.
* Use the this variable within methods so you can access the object's properties and methods from inside.


















 































