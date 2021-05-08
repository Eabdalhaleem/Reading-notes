# Why Forms?
The best known form on the web is probably 
the search box that sits right in the middle of 
Google's homepage.In addition to enabling users to 
search, forms also allow users 
to perform other functions 
online. You will see formswhen registering as a member 
of a website, when shopping 
online, and when signing up for 
newsletters or mailing lists 

---------

## Form ControlsThere 
are several types of form controls that 
you can use to collect information from visitors 
to your site

## ADDING TEXT:

## Password input
Like a single line text box but it 
masks the characters entered.

## Text input (single-line)
Used for a single line of text such 
as email addresses and names.

## Text area (multi-line)
For longer areas of text, such as 
messages and comments

-------

## Making Choices:
**Radio buttons**
For use when a user must select 
one of a number of options.

**Checkboxes**
When a user can select and 
unselect one or more options.

**Drop-down boxes**
When a user must pick one of a 
number of options from a list
## Submitting Forms:

**Submit buttons**
To submit data from your form 
to another web page.

**Image buttons**
Similar to submit buttons but 
they allow you to use an image

## Uploading Files
**File upload**
Allows users to upload files 
(e.g. images) to a website

----------

## How Forms Work
A user fills in a form and then presses a button 
to submit the information to the server

* The name of each form 
control is sent to the 
server along with the 
value the user enters or 
selects

* The server processes 
the information using a 
programming language 
such as PHP, C#, VB.net, 
or Java. It may also store 
the information in a 
database.

* The server creates a new 
page to send back to the 
browser based on the 
information received

----

A form may have several form controls, each 
gathering different information. The server 
needs to know which piece of inputted data 
corresponds with which form element

To differentiate between various pieces of inputted data, information 
is sent from the browser to the server using name/value pairs. In this 
example, the form asks for the visitor's username and also for their 
favorite jazz musician. The name/value pairs sent to the server are:
**username=Ivy**
If the form control allows the 
user to enter text, then the value 
of the form control is whatever 
the user has typed in.
**vote=Herbie**
If the form control allows you 
to choose from a fixed set of 
answers (e.g. radio buttons, 
checkboxes or a drop down list), 
the web page author will add 
code that gives each option an 
automatic value.

You should never change the name of a form control in a page unless 
you know that the code on the server will understand this new value.

-----------

# Form Structure
`<form>`
Form controls live inside a 
`<form>` element. This element 
should always carry the action
attribute and will usually have a 
method and id attribute too.
**action**
Every `<form>` element requires 
an action attribute. Its value
is the URL for the page on the 
server that will receive the 
information in the form when it 
is submitted.
**method**
Forms can be sent using one of 
two methods: get or post.
With the get method, the values 
from the form are added to 
the end of the URL specified in 
the action attribute. The get
method is ideal for:
* short forms (such as search 
boxes)
* when you are just retrieving 
data from the web server 
(not sending information that 
should be added to or deleted 
from a database

With the post method the 
values are sent in what are 
known as HTTP headers. As a 
rule of thumb you should use the 
post method if your form:
* allows users to upload a file
* is very long
* contains sensitive data 
(e.g. passwords)
* adds information to, or 
deletes information from, a 
database
If the method attribute is not 
used, the form data will be sent 
using the get method.
**id**
 but the value is used to 
identify the form distinctly from 
other elements on the page (and 
is often used by scripts — such 
as those that check you have 
entered information into fields 
that require values

------

## Text Input
`<input>`
The `<input>` element is used 
to create several different form 
controls. The value of the type
attribute determines what kind 
of input they will be creating.
**type="text"**
When the type attribute has a 
value of text, it creates a singleline text input.

**name**
When users enter information 
into a form, the server needs to 
know which form control each 
piece of data was entered into. 
(For example, in a login form, the 
server needs to know what has 
been entered as the username 
and what has been given as the 
password.) Therefore, each form 
control requires a name attribute. 
The value of this attribute 
identifies the form control and is 
sent along with the information 
they enter to the server.

**maxlength**
You can use the maxlength
attribute to limit the number 
of characters a user may enter 
into the text field. Its value is the 
number of characters they may 
enter. For example, if you were 
asking for a year, the maxlength
attribute could have a value of 4


**size**
The size attribute should not 
be used on new forms. It was 
used in older forms to indicate 
the width of the text input 
(measured by the number of 
characters that would be seen). 
For example, a value of 3 would 
create a box wide enough to 
display three characters 
(although a user could enter 
more characters if they desired).
In any new forms you write, 
CSS should be used to control 
the width of form elements. 
The size attribute is only 
mentioned here because you 
may come across it when looking 
at older code.


----------

## Password Input

`<input>`
**type="password"**
When the type attribute has 
a value of password it creates 
a text box that acts just like a 
single-line text input, except 
the characters are blocked out. 
They are hidden in this way so 
that if someone is looking over 
the user's shoulder, they cannot 
see sensitive data such as 
passwords.

**name**
The name attribute indicates 
the name of the password input, 
which is sent to the server with 
the password the user enters.

**size, maxlength**
It can also carry the size and 
maxlength attributes like the 
the single-line text input

-------- 

## Text Area

`<textarea>`
The `<textarea> `element 
is used to create a mutli-line 
text input. Unlike other input 
elements this is not an empty 
element. It should therefore have 
an opening and a closing tag. 
Any text that appears between 
the opening `<textarea>` and 
closing `</textarea>` tags will 
appear in the text box when the 
page loads.
If the user does not delete any 
text between these tags, this 
message will get sent to the 
server along with whatever the 
user has typed. (Some sites 
use JavaScript to clear this 
information when the user clicks 
in the text area.

----------

## Radio Button

`<input>`
**type="radio"**
Radio buttons allow users to pick 
just one of a number of options. 

**name**
The name attribute is sent to 
the server with the value of the 
option the user selects. When 
a question provides users with 
options for answers in the form 
of radio buttons, the value of 
the name attribute should be the 
same for all of the radio buttons 
used to answer that question. 

**value**
The value attribute indicates 
the value that is sent to the 
server for the selected option. 
The value of each of the buttons 
in a group should be different 
(so that the server knows which 
option the user has selected).

**checked**
The checked attribute can be 
used to indicate which value (if 
any) should be selected when 
the page loads. The value of this 
attribute is checked. Only one 
radio button in a group should 
use this attribute

---------

## Checkbox

`<input>`
type="checkbox"
Checkboxes allow users to select 
(and unselect) one or more 
options in answer to a question.

**name**
The name attribute is sent to 
the server with the value of the 
option(s) the user selects. When 
a question provides users with 
options for answers in the form 
of checkboxes, the value of the 
name attribute should be the 
same for all of the buttons that 
answer that question.

**value**
The value attribute indicates 
the value sent to the server if this 
checkbox is checked.

**checked**
The checked attribute indicates 
that this box should be checked 
when the page loads. If used, its 
value should be checked

---------

## Drop Down List Box

`<select>`
A drop down list box (also 
known as a select box) allows 
users to select one option from a 
drop down list. 
The `<select> `element is used 
to create a drop down list box. It 
contains two or more `<option>`
elements.

**name**
The name attribute indicates the 
name of the form control being 
sent to the server, along with the 
value the user selected.
`<option>`
The `<option>` element is used 
to specify the options that the 
user can select from. The words 
between the opening `<option>`
and closing `</option>` tags will 
be shown to the user in the drop 
down box.
**value**
The `<option>` element uses the 
value attribute to indicate the 
value that is sent to the server 
along with the name of the 
control if this option is selected.

**Drop Down List Box**
**selected**
The selected attribute can be 
used to indicate the option that 
should be selected when the 
page loads. The value of this 
attribute should be selected.
If this attribute is not used, 
the first option will be shown 
when the page loads. If the user 
does not select an option, then 
the first item will be sent to 
the server as the value for this 
control

------------

## Multiple Select Box

`<select>`
**size**
You can turn a drop down select 
box into a box that shows more 
than one option by adding the 
size attribute. Its value should 
be the number of options you 
want to show at once. In the 
example you can see that three 
of the four options are shown.
Unfortunately, the way that 
browsers have implemented this 
attribute is not perfect, and it 
should be tested throroughly if 
used (in particular in Firefox and 
Safari on a Mac).

**multiple**
You can allow users to select 
multiple options from this list by 
adding the multiple attribute 
with a value of multiple. 
It is a good idea to tell users if 
they can select more than one 
option at a time. It is also helpful 
to indicate that on a PC they 
should hold down the control key 
while selecting multiple options 
and on a Mac they should use 
the command key while selecting 
options.

----------

## File Input Box
`<input>`
If you want to allow users to 
upload a file (for example an 
image, video, mp3, or a PDF), 
you will need to use a file input 
box.
**type="file"**
This type of input creates a 
box that looks like a text input 
followed by a browse button. 
When the user clicks on the 
browse button, a window opens 
up that allows them to select a 
file from their computer to be 
uploaded to the website

--------

## Submit Button
`<input>`
type="submit"
The submit button is used to 
send a form to the server.

**name**
It can use a name attribute but it 
does not need to have one.

**value**
The value attribute is used to 
control the text that appears 
on a button. It is a good idea to 
specify the words you want to 
appear on a button because the 
default value of buttons on some 
browsers is ‘Submit query’ and 
this might not be appropriate for 
all kinds of form.

-------

## Image Button

`<input>`
**type="image"**
If you want to use an image for 
the submit button, you can give 
the type attribute a value of 
image. The src, width, height, 
and alt attributes work just 
like they do when used with the 
`<img>` element 

------------

## Button & hidden Controls

`<button>`
The `<button>` element was 
introduced to allow users more 
control over how their buttons 
appear, and to allow other 
elements to appear inside the 
button.
This means that you can 
combine text and images 
between the opening `<button>`
tag and closing `</button>` tag.

`<input>`
**type="hidden"**
This example also shows a 
hidden form control. These form 
controls are not shown on the 
page (although you can see them 
if you use the View Source option 
in the browser). They allow web 
page authors to add values to 
forms that users cannot see. 
For example, a web page author 
might use a hidden field to 
indicate which page the user was 
on when they submitted a form.

----------- 

## Labelling Form Controls

`<label>`
When introducing form controls, 
the code was kept simple by 
indicating the purpose of each 
one in text next to it. However, 
each form control should have

its own `<label>` element as this 
makes the form accessible to 
vision-impaired users.
The `<label>` element can be 
used in two ways. It can:
* Wrap around both the text 
description and the form input 
(as shown on the first line of the 
example to your right).
* Be kept separate from the 
form control and use the for
attribute to indicate which form 
control it is a label for (as shown 
with the radio buttons).

**for**
The for attribute states which 
form control the label belongs to. 
Note how the radio buttons use 
the id attribute. The value of the 
id attribute uniquely identifies an 
element from all other elements 
on a page.
The value of the for attribute 
matches that of the id attribute 
on the form control it is labelling.
This technique using the for and 
id attributes can be used on any 
form control. When a `<label>`
element is used with a checkbox 
or radio button, users can click 
on either the form control or the 
label to select. The expanded 
clickable area makes the form 
easier to use. The position of the 
label is very important. If users 
do not know where to enter 
information or what information 
to enter, they are less likely to 
use the form correctly. 
As a rule of thumb, here are the 
best places to place labels on 
form controls.
**Above or to the left:**
* Text inputs
* Text areas
* Select boxes
* File uploads
**To the right:**
* Individual checkboxes
* Individual radio button

-------------

## Grouping Form Elements

`<fieldset>`
You can group related form 
controls together inside the 
`<fieldset>` element. This is 
particularly helpful for longer 
forms.
Most browsers will show the 
fieldset with a line around 
the edge to show how they are 
related. The appearance of these 
lines can be adjusted using CSS.
`<legend>`
The `<legend>` element can 
come directly after the opening 
`<fieldset>` tag and contains a 
caption which helps identify the 
purpose of that group of form 
controls.

---------

## Form Validation

You have probably seen forms 
on the web that give users 
messages if the form control has 
not been filled in correctly; this is 
known as form validation.
Traditionally, form validation 
has been performed using 
JavaScript (which is beyond the 
scope of this book). But HTML5 
is introducing validation and 
leaving the work to the browser.
Validation helps ensure the 
user enters information in a 
form that the server will be able 
to understand when the form 
is submitted. Validating the 
contents of the form before it is 
sent to the server the helps: 
* Reduce the amount of work 
the server has to do
* Enables users to see if there 
are problems with the form 
faster than if validation were 
performed on the server.

----------

## Date Input
`<input>`
Many forms need to gather 
information such as dates, email 
addresses, and URLs. This has 
traditionally been done using 
text inputs.
HTML5 introduces new form 
controls to standardize the 
way that some information is 
gathered. Older browsers that 
do not recognize these inputs 
will just treat them as a single 
line text box. 
**type="date"**
If you are asking the user for a 
date, you can use an `<input>`
element and give the type
attribute a value of date. 
This will create a date input in 
browsers that support the new 
HMTL5 input types.

---------

## Email & URL Input

`<input>`
HTML5 has also introduced 
inputs that allow visitors to 
enter email addresses and URLs. 
Browsers that do not support 
these input types will just treat 
them as text boxes.

**type="email"**
If you ask a user for an email 
address, you can use the email 
input. Browsers that support 
HTML5 validation will check 
that the user has provided 
information in the correct format 
of an email address. Some smart 
phones also optimize their 
keyboard to display the keys you 
are most likely to need when 
entering an email address (such 
as the @ symbol).

**type="url"**
A URL input can be used when 
you are asking a user for a web 
page address. Browsers that 
support HTML5 validation will 
check that the user has provided 
information in the format of 
a URL. Some smart phones 
also optimize their keyboard to 
display the keys you are most 
likely to need when entering a 
URL

-----------

## Search Input
`<input>`
If you want to create a single 
line text box for search queries, 
HTML5 provides a special type 
of input for that purpose.

**type="search"**
If you want to create a single 
line text box for search queries, 
HTML5 provides a special 
search input.

To create the HTML5 search box 
the `<input>` element should 
have a type attribute whose 
value is search. Older browsers 
will simply treat it like a single 
line text box.

Recent browsers add some 
features that improve usability. 
For example, Safari on a Mac 
adds a cross to clear the search 
box when you have started to 
enter information. Safari also 
automatically rounds the corners 
on the search input field.

**placeholder**
On any text input, you can 
also use an attribute called 
placeholder whose value is 
text that will be shown in the 
text box until the user clicks in 
that area. Older browsers simply 
ignore this attribute

--------

* Whenever you want to collect information from 
visitors you will need a form, which lives inside a 
`<form>` element.
* Information from a form is sent in name/value pairs.
* Each form control is given a name, and the text the 
user types in or the values of the options they select 
are sent to the server.
* HTML5 introduces new form elements which make it 
easier for visitors to fill in forms

-------------

## Bullet Point Styles
**list-style-type**

The list-style-type property 
allows you to control the shape 
or style of a bullet point (also 
known as a marker). 
It can be used on rules that 
apply to the `<ol>`, `<ul>`, and `<li>`
elements.
Unordered Lists
For an unordered list you can use 
the following values:
 none
 disc
 circle
 square
Ordered Lists
For an ordered (numbered) list 
you can use the following values:
decimal
1 2 3
decimal-leading-zero
01 02 03
lower-alpha
a b c
upper-alpha
A B C
lower-roman
i. ii. iii.
upper-roman 
I II II

------------

## Images for Bullets
**list-style-image**

You can specify an image to act 
as a bullet point using the
list-style-image property.
The value starts with the letters 
url and is followed by a pair 
of parentheses. Inside the 
parentheses, the path to the 
image is given inside double 
quotes.
This property can be used on 
rules that apply to the `<ul> `and 
`<li>` elements.
The example on this page also 
shows the use of the margin
property to increase the vertical 
gap between each item in the 
list

--------------


## Positioning the Marker
**list-style-position**

Lists are indented into the page 
by default and the list-styleposition property indicates 
whether the marker should 
appear on the inside or the 
outside of the box containing the 
main points. 
This property can take one of 
two values:

**outside**
The marker sits to the left of the 
block of text. (This is the default 
behaviour if this property is not 
used.) 

**inside**

The marker sits inside the box of 
text (which is indented).
In the example shown, the width 
of the list has been limited to 150 
pixels. This ensures that the text 
wraps onto a new line so you can 
see how the value of inside sits 
the bullet inside the first line of 
text. 
A margin has been added to 
each list item so that there is a 
clear gap between each

---------

## List Shorthand

**list-style**
As with several of the other CSS 
properties, there is a property 
that acts as a shorthand for list 
styles. It is called list-style, 
and it allows you to express 
the markers' style, image and 
position properties in any order.

-------


## Table Properties
You have already met several 
properties that are commonly 
used with tables. Here we will 
put them together in a single 
example using the following:
width to set the width of the 
table

**padding** to set the space 
between the border of each table 
cell and its content

**text-transform**to convert the 
content of the table headers to 
uppercase

**letter-spacing, font-size**
to add additional styling to the 
content of the table headers
border-top, border-bottom
to set borders above and below 
the table headers

**text-align** to align the writing 
to the left of some table cells and 
to the right of the others

**background-color** to change 
the background color of the 
alternating table rows

**:hover**to highlight a table row 
when a user's mouse goes over it

Here are some tips for styling 
tables to ensure they are clean 
and easy to follow:

**Give cells padding**

If the text in a table cell either 
touches a border (or another 
cell), it becomes much harder to 
read. Adding padding helps to 
improve readability.

**Distinguish headings**
Putting all table headings in 
bold (the default style for the 
`<th>` element) makes them 
easier to read. You can also 
make headings uppercase and 
then either add a background 
color or an underline to clearly 
distinguish them from content.

**Shade alternate rows**
Shading every other row can 
help users follow along the lines. 
Use a subtle distinction from the 
normal color of the rows to keep 
the table looking clean.

**Align numerals**
You can use the text-align
property to align the content 
of any column that contains 
numbers to the right, so that 
large numbers are clearly 
distinguished from smaller ones.

**Online extra**
There are more examples of 
using CSS to style tables in the 
tools section of the website.

---------

## Border on Empty Cells
**empty-cells**
If you have empty cells in 
your table, then you can use 
the empty-cells property to 
specify whether or not their 
borders should be shown.
Since browsers treat empty cells 
in different ways, if you want to 
explicitly show or hide borders 
on any empty cells then you 
should use this property.
It can take one of three values:

**show**
This shows the borders of any 
empty cells.

**hide**
This hides the borders of any 
empty cells.

**inherit**
If you have one table nested 
inside another, the inherit
value instructs the table cells to 
obey the rules of the containing 
table.

In the first table on the left, you 
can see that the border of the 
empty cell is showing. In the 
second table, it is hidden.

----------

## Gaps Between Cells
**border-spacing, border-collapse**
The border-spacing property 
allows you to control the 
distance between adjacent cells. 
By default, browsers often leave 
a small gap between each table 
cell, so if you want to increase 
or decrease this space then 
the border-spacing property 
allows you to control the gap.

The value of this property is 
usually specified in pixels. You 
can specify two values if desired 
to specify separate numbers for 
horizontal and vertical spacing.

When a border has been used 
on table cells, where two cells 
meet, the width of lines would be 
twice that of the outside edges. 
It is possible to collapse adjacent 
borders to prevent this using the 
border-collapse property. 
Possible values are:

**collapse**
Borders are collapsed into a 
single border where possible. 
(border-spacing will be 
ignored and cells pushed 
together, and empty-cells
properties will be ignored.)

**separate**
Borders are detached from each 
other. (border-spacing and 
empty-cells will be obeyed.)

----------

## Styling Forms

Nobody I know enjoys filling 
in forms, so if you can make 
yours look more attractive and 
easier to use, more people are 
likely to fill it in. Also, when you 
come to look at a form in a few 
different browsers (as shown 
on the right), you will see that 
each browser displays them 
differently.

CSS is commonly used to 
control the appearance of form 
elements. This is both to make 
them more attractive and to 
make them more consistent 
across different browsers
 It is most common to style:
* Text inputs and text areas
* Submit buttons
* Labels on forms, to get the 
form controls to align nicely
In the coming pages you will see 
how to control these with CSS.
Mac: Safari Mac: Firefox
Pc: Chrome Pc: IE
Styling text inputs and submit 
buttons is fairly easy. It is 
harder to get select boxes, radio 
buttons, and checkboxes to look 
consistent across all browsers. 

--------

## Styling Text Inputs

This example demonstrates the 
CSS properties commonly used 
with text inputs, most of which 
you have already met. 

**font-size**sets the size of the 
text entered by the user.
**color** sets the text color, and 
**background-color** sets the 
background color of the input.

**border**adds a border around 
the edge of the input box, and
**border-radius** can be used 
to create rounded corners (for 
browsers that support this 
property).

The **:focus** pseudo-class is 
used to change the background 
color of the text input when it 
is being used, and the :hover
psuedo-class applies the same 
styles when the user hovers over 
them.

**background-image** adds a 
background image to the box. 
Because there is a different 
image for each input, we are 
using an attribute selector 
looking for the value of the id
attribute on each input.

--------
## Styling Submit Buttons

Here are some properties that 
can be used to style submit 
buttons. This example builds 
on the one in the previous page, 
and the submit button inherits 
the styles set for the `<input>`
element on the last page.
**color** is used to change the 
color of the text on the button.

**text-shadow** can give a 3D 
look to the text in browsers that 
support this property.

**border-bottom** has been used 
to make the bottom border of 
the button slightly thicker, which 
gives it a more 3D feel.

**background-color** can make 
the submit button stand out 
from other items around it. 

(Creating a consistent style 
for all buttons helps users 
understand how they should 
interact with the site.) A gradient 
background has been added for 
browsers that support gradients. 

The **:hover** pseudo-class 
has been used to change the 
appearance of the button when 
the user hovers over it. In this 
case, the background changes, 
the text gets darker, and the 
thicker border is applied to the 
top of the button

-----------

## Styling Fieldsets & Legends

Fieldsets are particularly helpful 
in determining the edges of a 
form. In a long form they can 
help group together related 
information within it.
The legend is used to indicate 
what information is required in 
the fieldset.
Properties commonly used with 
these two elements include:

**width**is used to control 
the width of the fieldset. In 
this example, the width of 
the fieldset forces the form 
elements to wrap onto a new line 
in the correct place. (If it were 
wider, the items might sit on one 
line.)
**color** is used to control the 
color of text.

**background-color** is used to 
change the color behind these 
items.

**border** is used to control the 
appearance of the border around 
the fieldset and/or legend.
**border-radius** is used to 
soften the edges of these 
elements in browsers that 
support this property.

**padding** can be used to add 
space inside these elements.

--------------

## Cursor Styles
 **Cursor**

 The cursor property allows 
you to control the type of mouse 
cursor that should be displayed 
to users.
For example, on a form you 
might set the cursor to be a hand 
when the user hovers over it. 
Here are the most commonly 
used values for this property:
* auto
* crosshair
* default
* pointer
* move
* text
* wait
* help
* url("cursor.gif");
You should only use these values 
to add helpful information for 
users in places they would 
expect to see that cursor. (For 
example, using a crosshair on a 
link might confuse users because 
they are not used to seeing it.)


---------
* In addition to the CSS properties covered in other 
chapters which work with the contents of all elements, 
there are several others that are specifically used to 
control the appearance of lists, tables, and forms.
* List markers can be given different appearances 
using the list-style-type and list-style image 
properties.
* Table cells can have different borders and spacing in 
different browsers, but there are properties you can 
use to control them and make them more consistent. 
* Forms are easier to use if the form controls are 
vertically aligned using CSS.
* Forms benefit from styles that make them feel more 
interactive

-------------

# DIFFERENT EVENT TYPES

![event](https://image.slidesharecdn.com/javascripteventhandler-130206005809-phpapp02/95/javascript-event-handler-6-638.jpg?cb=1360112430)


## TERMINOLOGY 
**EVENTS FIRE OR ARE RAISED**
When an event has occurred, it is often described as having fired or 
been raised. In the diagram on the right, if the user is tapping on a link, a 
click event would fire in the browser.

**EVENTS TRIGGER SCRIPTS**
Events are said to trigger a function or script. When the click event 
fires on the element in this diagram, it could trigger a script that enlarges 
the selected item

-------

# HOW EVENTS TRIGGER JAVASCRIPT CODE 
When the user interacts with the HTML on a web page, there are three 
steps involved in getting it to trigger some JavaScript code. 
Together these steps are known as event handling. 

* Select t he element 
node(s) you want the 
script to respond to. 
For example, if you want to 
trigger a function when a user 
clicks on a specific link, you need 
to get the DOM node for that 
link element. You do this using a 
DOM query .

* Indicate which event on 
the selected node(s) will 
trigger the response. 
Programmers call this binding an 
event to a DOM node. 
The previous two pages showed 
a selection of the popular events 
that you can monitor for. 

* State the code you want 
to run when the event 
occurs. 
When the event occurs, on a 
specified element, it will trigger 
a function. This may be a named 
or an anonymous function. 

-----
Here you can see how event handling can be used to provide feedback to 
users filling in a registration form. It will show an error message if their 
username is too short. 

* SELECT ELEMENT 
The element that users are 
interacting with is the text input 
where they enter the username.

* SPEC!FY EVENT 
When users move out of the 
text input, it loses focus, and the 
blur event fires on this element. 

* CALL CODE 
When the blur event fires 
on the username input, it 
will trigger a function called 
chec kUsername ().This function 
checks if the username is less 
than 5 characters. 
If there are not enough 
characters, it shows an error 
message that prompts the user 
to enter a longer username. 
If there are enough characters, 
the element that holds the error 
message should be cleared. 
This is because an error 
message may have been shown 
to the user already and they 
subsequently corrected their 
mistake. (If the error message 
was still visible when they had 
filled in the form correctly, it 
would be confusing.) 

-------

# THREE WAYS TO BIND AN EVENT TO AN ELEMENT



Event handlers let you indicate which event you 
are waiting for on any particular element. 
There are three types of event handlers. 

**HTML EVENT HANDLERS**
 
This is bad practice, but you 
need to be aware of it because 
you may see it in older code. 
Early versions of HTML included 
a set of attributes that could 
respond to events on the 
element they were added to. 
The attribute names matched 
the event names. Their values 
called the function that was to 
run when that event occurred. 
For example, the following: 
`<a onclick="hide()">` 
indicated that when a user 
clicked on this `<a>` element, the 
hi de () function would be called. 
This method of event handling 
is no longer used because it is 
better to separate the JavaScript 
from the HTML. You should use 
one of the other approaches 
shown on this page instead

**TRADITIONAL DOM EVENT HANDLERS** 
 
DOM event handlers were 
introduced in the original 
specification for the DOM. 
They are considered better than 
HTML event handlers because 
they let you separate the 
JavaScript from the HTML. 
Support in all major browsers is 
very strong for this approach. 
The main drawback is that you 
can only attach a single function 
to any event. For example, the 
submit event of a form cannot 
trigger one function that checks 
the contents of a form, and a 
second to submit the form data if 
it passes the checks. 
As a result of this limitation, if 
more than one script is used on 
the same page, and both scripts 
respond to the same event, then 
one or both of the scripts may 
not work as intended.

**DOM LEVEL 2 EVENT LISTENERS**

Event listeners were introduced 
in an update to the DOM 
specification (DOM level 2, 
released in the year 2000). 
They are now the favored way of 
handling events. 
The syntax is quite different and, 
unlike traditional event handlers, 
these newer event listeners allow 
one event to trigger multiple 
functions. As a result, there 
are less likely to be conflicts 
between different scripts that 
run on the same page. 

------

**HTML EVENT HANDLER ATTRIBUTES (DO NOT USE)** 
Please note: This approach is 
now considered bad practice; 
however, you need to be aware 
of it because you may see it if 
you are looking at older code. 
 
In the HTML, the first `<input>` 
element has an attribute called 
onb l ur (triggered when the user 
leaves the element). The value of 
the attribute is the name of the 
function that it should trigger. 
The value of the event handler 
attributes would be JavaScript. 
Often it would call a function 
that was written either in the 
`<head>` element or a separate

----------

# TRADITIONAL DOM EVENT HANDLERS 
All modern browsers understand this way of creating an event handler, 
but you can only attach one function to each event handler. 
Here is the syntax to bind an event to an element using an event handler, 
and to indicate which function should execute when that event fires:

**element .onevent functionName ;**
**ELEMENT.  EVENT .   CODE** 
DOM element Event bound to node(s) Name of function to call (with 
node to target preceded by word "on" no parentheses following it)

-------

**USING DOM EVENT HANDLERS**
In this example, the event 
handler appears on the last line 
of the JavaScript. Before the 
DOM event handler, two things 
are put in place:

*  If you use a named function 
when the event fires on your 
chosen DOM node, write that 
function first. (You could also 
use an anonymous function.)

* 2. The DOM element node is 
stored in a variable. Here the text 
input (whose id attribute has a 
value of username) is placed into 
a variable called e 1 Username. 

---

Event listeners are a more recent approach to handling events. 
They can deal with more than one function at a time 
but they are not supported in older browsers.

---

**USING PARAMETERS WITH EVENT HANDLERS & LISTENERS** 
Because you cannot have parentheses after the 
function names in event handlers or listeners, 
passing arguments requires a workaround. 

Usually, when a function needs 
some information to do its job, 
you pass arguments within the 
parentheses that follow the 
function name. 

When the interpreter sees the 
parentheses after a function call, 
it runs the code straight away. 
In an event handler, you want it 
to wait until the event triggers it. 

Therefore, if you need to pass 
arguments to a function that is 
called by an event handler or 
listener, you wrap the function 
call in an anonymous function.


---------

## USING PARAMETERS WITH EVENT LISTENERS 
The first line of this example shows the updated 
checkUsername() function. The mi nlength 
parameter specifies the minimum number of 
characters that the username should be. 

The value that is passed into the checkUsername() 
function is used in the conditional statement to 
check if the name is long enough, and provide 
feedback if the username name is too short. 

----

# Event Flow
Html elements nest inside other element .if you hover or click on a link,you will also  hovering or clicking on its patents.

## Why flow matters
the flow of events only  really matters when your code.has event handlers on an element and one of its ancestor or descendat elements.

-----

## The event object

When an event occurs, the event object tells 
you information about the event, and the 
element it happened upon.

Every time an event fires, the The event object is passed to 
event object contains helpful any function that is the event 
data about the event, such as: handler or listener.

* Which element the event happened on If you need to pass arguments 
* Which key was pressed for a to a named function, the event 
keypress event object will first be passed to the 
* What part of the viewport the anonymous wrapper function 
user clicked for a c 1 i ck event (this happens automatically); 
(the viewport is the part of then you must specify it as a 
the browser window that parameter of the named function 
shows the web page) (as shown on the next page).

-----

# EVENT DELEGATION 
Creating event listeners for a lot of elements 
can slow down a page, but event flow allows 
you to listen for an event on a parent element.

---

## CHANGING DEFAULT BEHAVIOR 

**preventDefau1t ()** 
Some events, such as clicking on 
links and submitting forms, take 
the user to another page. 
To prevent the default behavior 
of such elements (e.g., to keep 
the user on the same page 
rather than following a link 
or being taken to a new page 
after submitting a form), you 
can use the event object's 
preventoefault() method. 
IES- 8 have an equivalent 
property called return Va 1 ue 
which can be set to fa 1 se. A 
conditional statement can check 
if the prevent Def au 1t () method 
is supported, and use IE8's 
approach if it isn't: 
if (event .preventDefault) 
event.preventDefaul t (); 
else { 
event .returnVal ue = false; 
The event object has methods that change: 
the default behavior of an element and how 
the element's ancestors respond to the event.

* **stopPropagation()** 
Once you have handled an 
event using one element, you 
may want to stop that event 
from bubbling up to its ancestor 
elements (especially if there 
are separate event handlers 
responding to the same events 
on the containing elements). 
To stop the event bubbling up, 
you can use the event object's 
stopPropogation() method. 

**USING BOTH METHODS** 
You will sometimes see the 
following used in similar 
situations that are in a function: 
r eturn false; 
It prevents the default behavior 
of the element, and prevents 
the event from bubbling up or 
capturing further. It also works in 
all browsers, so it is popular.

 **USING EVENT DELEGATION**

-----

**WHICH ELEMENT DID ANEVENT OCCUR ON?**
When calling a function, the event object's target property is the best 
way to determine which element the event occurred on. But you may see 
the approach below used; it relies on the this keyword.

----

## DIFFERENT TYPES OF EVENTS 
In the rest of the chapter, you learn about the 
different types of events you can respond to. 

Events are defined in: 
* The W3C DOM specification 
* The HTMLS specification 
* In Browser Object Models

Most are a result of the user 
interacting with the HTML, but 
there are a few that react to the 
browser or other DOM events. 
We do not show every event, 
but the examples you see should 
teach you enough so that you 
can work with all types of events. 

-----

**USER INTERFACE EVENTS** 
User interface CUI) events occur as a result of interaction with the 
browser window rather than the HTML page contained within it, 
e.g., a page having loaded or the browser window being resized. 

The event handler I listener for 
UI events should be attached to 
the browser window. 
In old HTML code, you may see these events used as attributes on the 
opening `<body>` tag. (For example, older code used the on 1 oad attribute 
to trigger code that would run when the page had loaded.) 

----

## LOAD 
The load event is commonly 
used to trigger scripts that 
access the contents of the page. 
In this example, a function called 
setup() gives focus to the text 
input when the page has loaded

The event is automatically raised 
by the window object when a 
page has finished loading the 
HTML and all of its resources: 
images, CSS, scripts (even third 
party content e.g .. banner ads). 

The setup() function would not 
work before the page has loaded 
because it relies on finding the 
element whose id attribute has 
a value of username, in order to 
give it focus. 

**FOCUS & BLUR EVENTS** 
The HTML elements you can interact with, such as links and form 
elements, can gain focus. These events fire when they gain or lose focus.

**FOCUS & BLUR**
**ti pUsername ()** is triggered 
when the text input gains focus. 
It changes the cl ass attribute 
of the element containing the 
message, and updates the 
contents of the element. 
**checkUsername ()** is triggered 
when the text input loses focus. 
It adds a message and changes 
the cl ass if the username is less 
than 5 characters; otherwise, it 
clears the message.

------

## MOUSE EVENTS 

The mouse events are fired when the mouse is moved and also when its 
buttons are clicked. 
All of the elements on a page support the mouse 
events, and all of these bubble. Note that actions are 
different on touchscreen devices. 
 
Preventing a default behavior can have unexpected 
results. E.g., a click event only fires when both the 
mousedown and mouseup event have fired. 

----

## CLICK 

The aim of this example is to use 
the c 1 i ck event to remove the 
big note that has been added to 
the middle of the page. But first, 
the script has to create that note. 

Because the note is over the 
top of the page, we only want 
to show it to users who have 
JavaScript enabled (otherwise 
they could not hide it). 
 
When the c 1 i ck event fires on 
the close link the di smi ssNote() 
function is called. This function 
will remove the note that was 
added by the same script.

-------

## Where events occur
the event object can tell you where the cursor was positioned when an event was triggered.

* screen 
the screen x and screen y properties indicate the position of the cursor within the entire screen on your montior ,

* Page 
the page x and page y  properties indicate the position of the curos within the entiere page .

* client 
the client x and client y properties of the cursir within the browser view port.

-----

## DETERMINING POSITION  

In this example, as you move 
your mouse around the screen, 
the text inputs across the top of 
the page are updated with the 
current mouse position. 
This demonstrates the three 
different positions you can 
retrieve when the mouse is 
moved or when one of the 
buttons is clicked

--------
## KEYBOARD EVENTS

The keyboard events are fired when a user interacts with the keyboard 
(they fire on any kind of device with a keyboard). 

------

## FORM EVENTS
There are two events that are commonly used with forms. 
In particular you are likely to see submit used in form validation.

----

## MUTATION EVENTS & OBSERVERS

Whenever elements are added to or removed from the DOM, its 
structure changes. This change triggers a mutation event. 
When your script adds or removes content from a 
page it is updating the DOM tree. There are many 
reasons why you might want to respond to the DOM 
tree being updated, for example, you might want to 
tell the user that the page had changed. 

------

* Events are the browser's way of indicating when 
something has happened (such as when a page has 
finished loading or a button has been clicked). 

* Binding is the process of stating which event you are 
waiting to happen, and which element you are waiting 
for that event to happen upon. 

* When an event occurs on an element, it can trigger a 
JavaScript function. When this function then changes 
the web page in some way, it feels interactive because 
it has responded to the user. 

* You can use event delegation to monitor for events 

* that happen on all of the children of an element. 
The most commonly used events are W3C DOM 
events, although there are others in the HTMLS 
specification as well as browser-specific events. 