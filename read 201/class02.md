# HTML Text, CSS Introduction, and Basic JavaScript Instructions
## Text

HTML elements are used to describe the structure of 
the page (e.g. headings, subheadings, paragraphs).

* They also provide semantic information (e.g. where 
emphasis should be placed, the definition of any 
acronyms used, when given text is a quotation)

----
## Heading :

HTML has six "levels" of 
headings:
`<h1>` is used for main headings
`<h2>` is used for subheadings
If there are further sections 
under the subheadings then the 
`<h3>` element is used, and so 
on...
 ---


 ## paragraphs 

 `<p>`
To create a paragraph, surround 
the words that make up the 
paragraph with an opening `<p>`
tag and closing `</p>` tag.


 ## Bold & Ilitic
 `<b>`
By enclosing words in the tags 
`<b>` and `</b>` we can make 
characters appear **bold**.
The `<b>` element also represents 
a section of text that would be 
presented in a visually different 
way (for example key words in a 
paragraph) although the use of 
the `<b>` element does not imply 
any additional meaning.
`<i>`
By enclosing words in the tags 
`<i>` and `</i>` we can make 
characters appear *italic*.

------

  # Superscript & Subscrip

  `<sup>`
The <sup> element is used 
to contain characters that 
should be superscript such 
as the suffixes of dates or 
mathematical concepts like 
raising a number to a power such 
as 22

`<sub>`
The `<sub>` element is used to 
contain characters that should 
be subscript. It is commonly 
used with foot notes or chemical 
formulas such as H2
0.


---------

## White Space

In order to make code easier to 
read, web page authors often 
add extra spaces or start some 
elements on new lines.
When the browser comes across 
two or more spaces next to each 
other, it only displays one space. 
Similarly if it comes across a line 
break, it treats that as a single 
space too. This is known as 
white space collapsing

  ----
  ## strong & Emphasis

  `<em>`
The `<em>` element indicates 
emphasis that subtly changes 
the meaning of a sentence.

`<strong>`
The use of the `<strong>`
element indicates that its 
content has strong importance.

----------

# Quotations

There are two elements 
commonly used for marking up 
quotations:

`<blockquote>`

The `<blockquote>` element is 
used for longer quotes that take 
up an entire paragraph. Note 
how the `<p>` element is still 
used inside the `<blockquote>`
element. 

Browsers tend to indent the 
contents of the `<blockquote>`
element, however you should not 
use this element just to indent a 
piece of text — rather you should 
achieve this effect using CSS. 

`<q>`

The `<q>` element is used for 
shorter quotes that sit within 
a paragraph. Browsers are 
supposed to put quotes around 
the `<q>` element, however 
Internet Explorer does not — 
therefore many people avoid 
using the `<q>` element.

-------------

## Abbreviations & Acronyms

`<abbr>`
If you use an abbreviation or 
an acronym, then the `<abbr>`
element can be used. A title
attribute on the opening tag is 
used to specify the full term

---------
# Citations & Definitions

`<cite>`
When you are referencing a 
piece of work such as a book, 
film or research paper, the 
`<cite>` element can be used 
to indicate where the citation is 
from.
In HTML5, `<cite>` should not 
really be used for a person's 
name — but it was allowed in 
HTML 4, so most people are 
likely to continue to use it.
Browsers will render the content 
of a `<cite>` element in italics.

----
# Author Details

`<address>` 

The `<address>` element has 
quite a specific use: to contain 
contact details for the author of 
the page.

It can contain a physical address, 
but it does not have to. For 
example, it may also contain a 
phone number or email address.

-----
`<dfn>`
The first time you explain some 
new terminology (perhaps an 
academic concept or some 
jargon) in a document, it is 
known as the defining instance 
of it.
The `<dfn>` element is used to 
indicate the defining instance of 
a new term

-----
# Changes to Content
`<ins>`
`<del>`
The `<ins>` element can be used 
to show content that has been 
inserted into a document, while 
the `<del>` element can show text 
that has been deleted from it.
The content of a `<ins>` element 
is usually underlined, while the 
content of a `<del>` element 
usually has a line through it.

`<s>`
The `<s>` element indicates 
something that is no longer 
accurate or relevant (but that 
should not be deleted).
Visually the content of an `<s>`
element will usually be displayed 
with a line through the center.

--------

* HTML elements are used to describe the structure of 
the page (e.g. headings, subheadings, paragraphs).

* They also provide semantic information (e.g. where 
emphasis should be placed, the definition of any 
acronyms used, when given text is a quotation).

-----------

![css](https://marketplace-cdn.atlassian.com/files/images/f7d3a59d-5680-4f27-bcce-54a0f6780820.png)

------

# INtroducing CSS :

CSS allows you to create rules that control the 
way that each individual box (and the contents 
of that box) is presented.
CSS works by associating rules with HTML elements. These rules govern 
how the content of specified elements should be displayed.
 A CSS rule contains two parts: a selector and a declaration.
CSS declarations sit inside curly brackets and each is made up of two 
parts: a property and a value, separated by a colon. You can specify 
several properties in one declaration, each separated by a semi-colon.

  **Using External CSS**
 `<link>` chapter-10/using-external-css.html HTML
The `<link>` element can be used 
in an HTML document to tell the 
browser where to find the CSS 
file used to style the page. 
< link href="css/styles.css" type="text/css"

**Using Internal CSS**

`<style>`
You can also include CSS rules 
within an HTML page by placing 
them inside a `<style>` element, 
which usually sits inside the 
`<head>` element of the page. 
  
 -----
 # JS 
 A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon. 
A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables.
When you write JavaScript, you have to tell the
interpreter every individual step that you want it to
perform. This sometimes involves more detail than
you might expect. 

**A variable** is a good name for this
concept because the data stored
in a variable can change (or vary)
each time a script runs.

JavaScript distinguishes between numbers,
strings, and true or false values known as
Booleans.
Once you have assigned a value
to a variable, you can then
change what is stored in the
variable later in the same script

--
## CREATING AN ARRAY
You create an array and give it
a name just like you would any
other variable (using the var
keyword followed by the name of
the array)
Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one). 

there are two condition :
evaluation condition
condition statment
 you can evalute a sitiuation by comparing one value to what you expect

 ![html](http://4.bp.blogspot.com/-4Y13ry3aGXc/VmA_aWYH0JI/AAAAAAAAHlE/zWzmDyw-zac/s640/logo_html5.png)

--------

# Decision making
there are often several places in a script where decisions are made that determine which lines of code should be run next .flowcharts can help you plan for these occasions.

in a flowchart, the diamond shape represents a point where a decision must be made and the code can take one of two different path.

----------

# evaluting conditions & conditional statment :
there are tow components to a decision :
* An expression is evaluated , which returns a value 
* A conditional statment says what to do in given situation.

* **evaluting conditions**
in order to make a decision , your code checks the current status of the script .

* **conditional statment**

a conditional statements is based on a concept of if/then/else; if a condition i met, then your code executes one or more statments,else your code does something diferents.

---------

## decision making 

there are often several places in a script where deisions are made that determin which lines of code should be run next .flowcharts can help you plan for these occasions.

----

## Evaluating conditions & conditional statements

there are two comonents to a decision 
* an expression is evaluted , which returns a value
* a conditional statement says what to do in a given situation.


![con](https://transang.me/content/images/2020/04/Screen-Shot-2020-04-05-at-12.03.48-PM.png)

----

## Comparison operators: Evaluating conditions

you can evaluate a situation by comparing one value in the script to what you expect it might be. the result will be a boolean :true or false.
**(==)is equal** to copare 2 values to see if they are the same
**(!=)is not equal** to copare 2 values (numbers, string or boalen) to  see if they are not the same
**(===)strict equal** to compare 2 value to check that both the data type and value are the same
**(!==)strict** not equal to compare 2 value to check that both the data type and value are not the same

---------

(>)greater than
(<)less than
(>=)greater than or equal
(<=)less than or equal

------

![read1](img/read21.PNG)
![read22](img/read22.PNG)
![read3](img/read23.PNG)
![read24](img/read24.PNG)
![read25](img/read25.PNG)
![read26](img/read26.PNG)
![read27](img/read27.PNG)
![read28](img/read28.PNG)
![read29](img/read29.PNG)


----------

* Conditional statements allow your code to make 
decisions about what to do next. 

* Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>) 
are used to compare two operands.

* Logical operators allow you to combine more than one 
 set of comparison operators. 

* if ... else statements allow you to run one set of code 
if a condition is true, and another if it is false. 

* switch statements allow you to compare a value 
against possible outcomes (and also provides a default 
 option if none match). 

* Data types can be coerced from one type to another. 
 All values evaluate to either truthy or falsy. 

* There are three types of loop: for, while, and 
do ... while. Each repeats a set of statements.


-------

## How to Write a Git Commit Message

Introduction: Why good commit messages matter
If you browse the log of any random Git repository, you will probably find its commit messages are more or less a mess
Which would you rather read?

The former varies in length and form; the latter is concise and consistent.
The former is what happens by default; the latter never happens by accident.

While many repositories’ logs look like the former, there are exceptions. The Linux kernel and Git itself are great examples. Look at Spring Boot, or any repository managed by Tim Pope.

The contributors to these repositories know that a well-crafted Git commit message is the best way to communicate context about a change to fellow developers (and indeed to their future selves). A diff will tell you what changed, but only the commit message can properly tell you why. 

-------

Style. Markup syntax, wrap margins, grammar, capitalization, punctuation. Spell these things out, remove the guesswork, and make it all as simple as possible. The end result will be a remarkably consistent log that’s not only a pleasure to read but that actually does get read on a regular basis.

Content. What kind of information should the body of the commit message (if any) contain? What should it not contain?

Metadata. How should issue tracking IDs, pull request numbers, etc. be referenced?

Fortunately, there are well-established conventions as to what makes an idiomatic Git commit message. Indeed, many of them are assumed in the way certain Git commands function. There’s nothing you need to re-invent. Just follow the seven rules below and you’re on your way to committing like a pro.

--------







