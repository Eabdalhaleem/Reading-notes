# lists
## Ordered Lists
`<ol>`
The ordered list is created with 
the `<ol>` element.
`<li>`
Each item in the list is placed 
between an opening `<li>` tag 
and a closing `</li>` tag. (The li
stands for list item.)

----
## Unordered lists
`<ul>`
The unordered list is created 
with the `<ul> `element.
`<li>`
Each item in the list is placed 
between an opening `<li>` tag 
and a closing `</li>` tag. (The li
stands for list item.

## Definition Lists
`<dl>`
The definition list is created with 
the `<dl>` element and usually 
consists of a series of terms and 
their definitions.
Inside the `<dl> `element you will 
usually see pairs of `<dt>` and 
`<dd>` elements.
`<dt>`
This is used to contain the term 
being defined (the definition 
term).
`<dd>`
This is used to contain the 
definition.

--------------

There are three types of HTML lists: ordered, 
unordered, and definition. 
* Ordered lists use numbers.
* Unordered lists use bullets.
* Definition lists are used to define terminology.
* Lists can be nested inside one another

----
##  Box Dimensions(width, height)
enough to hold its contents. To 
set your own dimensions for a 
box you can use the height and 
width properties.

The most popular ways to 
specify the size of a box are 
to use pixels, percentages, or 
ems. Traditionally, pixels have 
been the most popular method 
because they allow designers to 
accurately control their size.

---
## Limiting Width(min-width, max-width)
Some page designs expand and 
shrink to fit the size of the user's 
screen. In such designs, the 
min-width property specifies 
the smallest size a box can be 
displayed at when the browser 
window is narrow, and the 
max-width property indicates 
the maximum width a box can 
stretch to when the browser 
window is wide.

## Border, Margin & Padding
Every box has three available properties that 
can be adjusted to control its appearance:
* **Border:**
Every box has a border (even if 
it is not visible or is specified to 
be 0 pixels wide). The border 
separates the edge of one box 
from another.
* **Margin:**
Margins sit outside the edge 
of the border. You can set the 
width of a margin to create a 
gap between the borders of two 
adjacent boxes.
* **Padding:**
Padding is the space between 
the border of a box and any 
content contained within it. 
Adding padding can increase the 
readability of its contents

---

## CREATING AN ARRAY
You create an array and give it
a name just like you would any
other variable (using the var
keyword followed by the name of
the array).

Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one). 
The first lines of code on the left
create an array containing a list
of three colors. (The values can
be added on the same line or on
separate lines as shown here.) 

--------

A switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value. 
If you use a data type JavaScript did not expect,
it tries to make sense of the operation rather
than report an error. 
Due to type coercion, every value in JavaScript
can be treated as if it were true or false; and
this has some interesting side effects

**Falsy** values are treated as if they
are fa 1 se. The table to the left
shows a hi ghScore variable with
a series of values, all of which
are falsy. 
**Truthy** values are treated as if
they are true. Almost everything
that is not in the falsy table can
be treated as if it were true.

Logical operators are processed left to right.
They short-circuit (stop) as soon as they have a
result - but they return the value that stopped
the processing (not necessarily true or fa 1 se). 
Logical operators will not always
return true or false, because:

* They return the value that
stopped processing.

* That value might have been
treated as truthy or falsy
although it was not a Boolean. 

## LOOPS
loop check  a condition , if it return true . a code block will run then the condition will check again
A for loop is often used to loop through the items in an array. 
  
Conditional statements allow your code to make
decisions about what to do next.
Comparison operators **(===, ! ==, ==, ! =, <, >, <=, =>)**
are used to compare two operands.

Logical operators allow you to combine more than one
set of comparison operators.

if ... else statements allow you to run one set of code
if a condition is true, and another if it is false.

switch statements allow you to compare a value
against possible outcomes (and also provides a default
option if none match).

Data types can be coerced from one type to another.
All values evaluate to either truthy or falsy.
There are three types of loop: for, while, and
do ... while. Each repeats a set of statements. 

-------

Here are three points to consider when you 
are working with loops. Each is illustrated in 
examples on the following three pages.

**KEYWORDS**

You will commonly see these 
two keywords used with loops: 

**break** 

This keyword causes the 
termination of the loop and tells 
the interpreter to go onto the 
next statement of code outside 
of the loop. (You may also see it 
used in functions.)

**continue** 

This keyword tells the interpreter 
to continue with the current 
iteration, and then check the 
condition again. (If it is true, the 
code runs again.)

**LOOPS & ARRAYS** 

Loops are very helpful when 
dealing with arrays if you want to 
run the same code for each item 
in the array. 

For example, you might want 
to write the value of each item 
stored in an array into the page. 
*You may not know how many*
items will be in an array when 
writing a script, but. when the 
code runs, it can check the total 
number of items in a loop. That 
figure can then be used in the 
counter to control how many 
times a set of statements is run. 
*Once the loop has run the right* 
number of times, the loop stops. 

----------

**PERFORMANCE ISSUES** 
It is important to remember 
that when a browser comes 
across JavaScript, it will stop 
doing anything else until it has 
processed that script.

If your loop is dealing with only 
a small number of items, this 
will not be an issue. If, however, 
your loop contains a lot of items, 
it can make the page slower to 
load. 

If the condition never returns 
fa1se, you get what is commonly 
referred to as an infinite loop. 
The code will not stop running 
until your browser runs out of 
memory (breaking your script).

Any variable you can define 
outside of the loop and that 
does not change within the loop 
should be defined outside of it. 
If it were declared inside the 
loop, it would be recalculated 
every time the loop ran, 
needlessly using resources. 

**USING FOR LOOPS**

A for loop is often used to loop 
through the items in an array. 
In this example, the scores for 
each round of a test are stored in 
an array called scores. 

The total number of items in 
the array is stored in a variable 
called arrayl ength. This 
number is obtained using the 
l ength property of the array. 

There are three more variables: 
roundNumber holds the round of 
the test; msg holds the message 
to display; i is the counter 
(declared outside the loop).

The loop starts with the for 
keyword, then contains the 
condition inside the parentheses.

As long as the counter is less 
than the total number of items 
in the array, the contents of the 
curly braces will continue to 
run. Each time the loop runs, the 
round number is increased by 1. 

Inside the curly braces are rules 
that write the round number and 
the score to the msg variable. The 
variables declared outside of the 
loop are used within the loop. 

The msg variable is then written 
into the page. It contains HTML 
so the i nnerHTML property is 
used to do this. Remember, 
p228 will talk about security 
issues relating to this property. 

----------

# USING WHILE LOOPS
Here is an example of awhil e 
loop. It writes out the 5 times 
table. Each time the loop is run, 
another calculation is written 
into the variable called msg.

This loop will continue to run 
for as long as the condition in 
the parentheses is true.
 That condition is a counter indicating 
that, as long as the variable 
i remains less than 10, the 
statements in the subsequent 
code block should run.

-------

# USING DO WHILE LOOPS

The key difference between 
a whi 1 e loop and a do whi 1 e 
loop is that the statements in 
the code block come before the 
condition. This means that those 
statements are run once whether 
or not the condition is met.

If you take a look at the 
condition, it is checking that the 
value of the variable called i is 
less than 1, but that variable has 
already been set to a value of 1. 

![loops](https://cdn.educba.com/academy/wp-content/uploads/2019/10/For-Loop-in-JavaScript.png)

-----------

* A script is made up of a series of statements. Each 
statement is like a step in a recipe. 
* Scripts contain very precise instructions. For example, 
* you might specify that a value must be remembered 
 before creating a calculation using that value. 
* Variables are used to temporarily store pieces of 
 information used in the script. 
* Arrays are special types of variables that store more 
than one piece of related information. 
* JavaScript distinguishes between numbers (0-9), 
strings (text), and Boolean values (true or false). 
* Expressions evaluate into a single value. 
* Expressions rely on operators to calculate a value.

---------

# if.. else statements

the if ..else statement checks a condition .
if it resolves to true the first code block is executed.
if the condition resolves to false the second code block is run instead .

![if](https://www.tutorialgateway.org/wp-content/uploads/JavaScript-If-Statement-2.png)

------

# USING IF ... ELSE STATEMENTS 


Here you can see that an 
if ... e1se statement allows you 
to provide two sets of code:

* one set if the condition 
evaluates to true 

* another set if the condition is 
false 

In this test, there are two 
possible outcomes: a user can 
either get a score equal to or 
greater than the pass mark 
(which means they pass), or 
they can score less than the pass 
mark (which means they fail). 
One response is required for 
each eventuality. T

-------

# SWITCH STATEMENTS

A switch statement starts with a 
variable called the switch value. 
Each case indicates a possible 
value for this variable and the 
code that should run if the 
variable matches that value. 

---------

# USING SWITCH STATEMENTS 

The variable called l eve 1 
contains a number indicating 
which level the user is on. This 
is then used as the switch value. 
(The switch value could also be 
an expression.

--------

# TYPE COERCION & WEAK TYPING
If you use a data type JavaScript did not expect, 
it tries to make sense of the operation rather 
than report an error.

# TRUTHY & FALSY VALUES 
Due to type coercion, every value in JavaScript 
can be treated as if it were true or false; and 
this has some interesting side effects.

**Falsy** values are treated as if they 
are fa 1 se. The table to the left 
shows a hi ghScore variable with 
a series of values, all of which 
are falsy. 

Falsy values can also be treated 
as the number 0 .

**Truthy** values are treated as if 
they are true. Almost everything 
that is not in the falsy table can 
be treated as if it were true.

Truthy values can also be treated 
as the number 1.

--------






























