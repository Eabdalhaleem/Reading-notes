# Tables
## What's a Table?

A table represents information in a grid format. 
Examples of tables include financial reports, TV 
schedules, and sports results

## Basic Table Structure

<table>
The <table> element is used 
to create a table. The contents 
of the table are written out row 
by row.


![tables](http://3.bp.blogspot.com/-m3yVfQjKy50/VWr2wjykduI/AAAAAAAAO-4/DEe2-YYq6Pw/s1600/HTML-table-shortcode.jpg)


------------

<tr>
You indicate the start of each 
row using the opening <tr> tag. 
(The tr stands for table row.) 
It is followed by one or more

-----------

<td> elements (one for each cell 
in that row). 
At the end of the row you use a 
closing </tr> tag.

------------

<td>
Each cell of a table is 
represented using a <td>
element. (The td stands for 
table data.)
At the end of each cell you use a 
closing </td> tag

------------

## Table Headings

<th>
The <th> element is used just 
like the <td> element but its 
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

<thead>
The headings of the table should 
sit inside the <thead> element. 

<tbody>
The body should sit inside the 
<tbody> element.

<tfoot>
The footer belongs inside the 
<tfoot> element

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
on the opening <table> tag to 
indicate how wide that table 
should be and on some opening 
<th> and <td> tags to specify 
the width of individual cells. 
The value of this attribute is 
the width of the table or cell in 
pixels.

The columns in a table need to 
form a straight line, so you often 
only see the width attribute on 
the first row (and all subsequent 
rows would use that setting).
The opening <table> tag could 
also use the cellpadding
attribute to add space inside 
each cell of the table, and the 
cellspacing attribute to create 
space between each cell of 
the table. The values for these 
attributes were given in pixels.

-----------

* The <table> element is used to add tables to a web 
page.

* A table is drawn out row by row. Each row is created 
with the <tr> element.

* Inside each row there are a number of cells 
represented by the <td> element (or <th> if it is a 
header).

* You can make cells of a table span more than one row 
or column using the rowspan and colspan attributes.

* For long tables you can split the table into a <thead>, 
<tbody>, and <tfoot>

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