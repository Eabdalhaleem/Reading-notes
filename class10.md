# Error Handling & Debugging

JavaScript can be hard to learn and everyone makes 
mistakes when writing it. This chapter will help you learn how to find the errors in your code. It will also teach you how to write scripts that deal with potential errors gracefully. 
When you are writing JavaScript, do not expect to write it perfectly the first time. 

Programming is like problem solving: you are given a puzzle and not only do you have to solve 
it, but you also need to create the instructions that allow the computer to solve it. too. 

When writing a long script, nobody gets everything right in their first attempt. The error 
messages that a browser gives look cryptic at first, but they can help you determine what 
went wrong in your JavaScript and how to fix it. In this chapter you will learn about:

**THE CONSOLE & DEV TOOLS** 
Tools built into the browser 
that help you hunt for errors. 
9 ERROR HANDLING & DEBUGGING 

**COMMON PROBLEMS** 
Common sources of errors, 
and how to solve them. 

**HANDLING ERRORS**
How code can deal with 
potential errors gracefully. 



![error](https://dab1nmslvvntp.cloudfront.net/wp-content/uploads/2016/04/1496946239error.jpg)


-------

## ORDER OF EXECUTION 
To find the source of an error, it helps to know how scripts are processed. 
The order in which statements are executed can be complex; some tasks 
cannot complete until another statement or function has been run

---

## EXECUT.ION CONTEXTS 
The JavaScript interpreter uses the concept of execution contexts. 
There is one global execution context; plus, each function creates a new 
new execution context. They correspond to variable scope. 

-------

## The Stack

the javascript interprete processes one line of code at a time . when a statement needs data from another function , it stacks (or piles )the new function on top of the current task.

----

**EXECUTION CONTEXT & HOISTING**
Each time a script enters a new execution context, there are two phases 
of activity: 
* **PREPARE** 
* The new scope is created 
* Variables, functions, and arguments are created 
* The value of the this keyword is determined

* **EXECUTE** 
* Now it can assign values to variables 
* Reference functions and run their code 
* Execute statements

-------

## UNDERSTANDING SCOPE 

In the interpreter, each execution context has its own va ri ables object. 
It holds the variables, functions, and parameters available within it. 
Each execution context can also access its parent's v ari ables object. 
Functions in JavaScript are said to have lexical scope. 
They are linked to the object they were defined within. 
So, for each execution context, the scope is the 
current execution context's variables object, plus the 
variables object for each parent execution context. 

------

## UNDERSTANDING ERRORS 
If a JavaScript statement generates an error, then it throws an exception. 
At that point, the interpreter stops and looks for exception-handl ing code. 

------
## ERROR OBJECTS

Error objects can help you find where your mistakes are 
and browsers have tools to help you read them.

## ERROR OBJECTS CONTINUED

**Syntax Error** 
SYNTAX IS NOT CORRECT 
This is caused by incorrect use of the rules of the 
language. It is often the result of a simple typo. 
**MISMATCHING OR UNCLOSED QUOTES**
document .write ("Howdyl ); 
SyntaxError: Unexpect ed EOF 

**MISSING CLOSING BRACKET** 
document .getElementByid('page' I 
SyntaxErr or : Expected token ' ) ' 

**MISSING COMMA IN ARRAY** 
Would be same for missing] at the end 
var l ist = ['Item 1', 'Item 2 ' l 'rtem 3']; 
SyntaxError: Expected token ']'

**MALFORMED PROPERTY NAME**
It has a space but is not surrounded by quote marks 
user = {f i rstl name: "Ben", lastName: "Lee"}; 

Synt axError: Expected an identifier but 
found 'name ' instead

**Ref erenceError** 
VARIABLE DOES NOT EXIST 
This is caused by a variable that is not declared or is 
out of scope. 

**VA RIABLE IS UNDECLARED** 
var wi dth = 12 ; 
var area = width * llt!ftNU! ; 
ReferenceError: Can ' t find vari able: 
height

**NAMED FUNCTION IS UNDEFINED** 
document.write ( randomFunction() ) ; 
ReferenceError: Can't find variable : 
randomFunction

--------

## HOW TO DEAL WITH ERRORS 
Now that you know what an error is and how the browser treats them, 
there are two things you can do with the errors. 

* **DEBUG THE SCRIPT TO FIX ERRORS** 
If you come across an error while writing a script 
(or when someone reports a bug), you will need to 
debug the code, track down the source of the error, 
and fix it. 

You will find that the developer tools available in 
every major modern browser will help you with 
this task. In this chapter, you will learn about the 
developer tools in Chrome and Firefox. (The tools in 
Chrome are identical to those in Opera.) 

IE and Safari also have their own tools (but there is 
not space to cover them all). 
 
* **HANDLE ERRORS GRACEFULLY** 
You can handle errors gracefully using try, catch, 
throw, and f i na 1 ly statements. 

Sometimes, an error may occur in the script for a 
reason beyond your control. For example, you might 
request data from a third party, and their server 
may not respond. In such cases, it is particularly 
important to write error-handling code. 

In the latter part of the chapter, you will learn how to 
gracefully check whether something will work, and 
offer an alternative option if it fails.

----------

## A DEBUGGING WORKFLOW

Debugging is about deduction: eliminating potential causes of an error. 
Here is a workflow for techniques you will meet over the next 20 pages. 
Try to narrow down where the problem might be, then look for clues. 

**WHERE IS THE PROBLEM?** 
First, should try to can narrow down the area where 
the problem seems to be. In a long script, this is 
especially important. 

**WHAT EXACTLY IS THE PROBLEM?** 
Once you think that you might know the rough area 
in which your problem is located, you can then try to 
find the actual line of code that is causing the error.

---------

## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE 
The JavaScript console will tell you when there is a problem with a script, 
where to look for the problem, and what kind of issue it seems to be. 
These two pages show instructions for opening the 
console in all of the main browsers (but the rest of 
this chapter will focus on Chrome and Firefox)

CHROM E/ OPERA 
On a PC, press the F12 key or: 
* Go to the options menu (or three line menu icon) 
* Select Toots or More tools. 
* Select JavaScript Console or Developer Tools 
On a Mac press Alt + Cmd + J. Or: 
* Go to the View menu. 
* Select Developer. 
* Open the JavaScript Console or Developer Tools 
option and select Console. 
INTERNET EXPLORER 
Press the F12 key or: 
* Go to the settings menu in the top-right. 
* Select developer tools.

-------

The JavaScript console is just one of several developer tools that are 
found in all modern browsers. 
When you are debugging errors, it can help if you 
look at the error in more than one browser as they 
can show you different error messages. 

If you open the errors . html file from t he sample 
code in your browser, and then open the console, 
you will see an error is displayed.

-------

**HOW TO LOOK AT ERRORS IN CHROME** 
The console will show you when there is an 
error in your JavaScript. It also displays the line 
where it became a problem for the interpreter. 

----

**WRITING FROM THE SCRIPT TO THE CONSOLE** 
Browsers that have a console have a console object, which has several 
methods that your script can use to display data in the console. 
The object is documented in the Console API.

-------

## LOGGING DATA TO THE CONSOLE 
This example shows several uses 
of the console . log () method. 

* The first line is used to indicate 
the script is running. 
* Next an event handler waits 
for the user leaving a text input, 
and logs the value that they 
entered into that form field. 
JAVASCRIPT 
When the user submits the form, 
four values are displayed: 

* That the user clicked submit 
* The value in the width input 
* The value in the height input 
* The value of the area variable 
They help check that you are 
getting the values you expect.

The console . log() method 
can write several values to the 
console at the same time, each 
separated by a comma, as shown 
when displaying the height (5). 
You should always remove this 
kind of error handling code from 
your script before you use it on 
a live site. 

------

## MORE CONSOLE METHODS 
To differentiate between the 
types of messages you write 
to the console, you can use 
three different methods. They 
use various colors and icons to 
distinguish them.

* conso1e. info() can be used 
for general information 
* console.warn() can be used 
for warnings 
* console.error() can be used 
to hold errors
This technique is particularly 
helpful to show the nature of the 
information that you are writing 
to the screen. (In Firefox, make 
sure you have the logging option 
selected.) 

-----

## GROUPING MESSAGES 
* If you want to write a set of 
related data to the console, you 
can use the console. group () 
method to group the messages 
together. You can then expand 
and contract the results. 
It has one parameter; the name 
that you want to use for the 
group of messages. You can 
then expand and collapse the 
contents by clicking next to the 
group's name as shown below. 

* When you have finished 
writing out the results for the 
group, to indicate the end of the 
group the console .groupEnd () 
method is used. 

------------

## WRITING TABULAR DATA 

In browsers that support it, the 
console. table () method lets 
you output a table showing: 
* objects 
* arrays that contain other 
objects or arrays

------

## WRITING ON A CONDITION

Using the console. assert() 
method, you can test if a 
condition is met, and write to the 
console only if the expression 
evaluates to false. 

----

## BREAKPOINTS 
You can pause the execution of a script on any 
line using breakpoints. Then you can check the 
values stored in variables at that point in time.

--------

## STEPPING THROUGH CODE 

If you set multiple breakpoints, you can step 
through them one-by-one to see where values 
change and a problem might occur.


-------

## CONDITIONAL BREAKPOINTS 
You can indicate that a breakpoint should be 
triggered only if a condition that you specify is 
met. The condition can use existing variables. 

-------

## DEBUGGER KEYWORD

You can create a breakpoint 
in your code using just the 
debugger keyword. When the 
developer tools are open, this 
will automatically create a 
breakpoint. 
You can also place the debugger 
keyword within a conditional 
statement so that it only triggers 
the breakpoint if the condition is 
met. 



1[er](https://image.slidesharecdn.com/error-handlinganddebugging-120524084901-phpapp02/95/error-handling-and-debugging-in-vb-2-728.jpg?cb=1337849468)


--------

## HANDLING EXCEPTIONS 
If you know your code might fail, use try, catch, and finally. 
Each one is given its own code block.

---

## TRY, CATCH, FINALLY


**TRY** 
First, you specify the code 
that you think might throw an 
exception within the try block. 
If an exception occurs in this 
section of code, control is 
automatically passed to the 
corresponding catch block. 
The try clause must be used in 
this type of error handling code, 
and it should always have either 
a catch, fi na 1 ly, or both. 
If you use a continue, break, or 
return keyword inside a try, it 
will go to the f i na 11 y option.

-----

**CATCH** 
If the try code block throws an 
exception, catch steps in with an 
alternative set of code. 
It has one parameter: the error 
object. Although it is optional, 
you are not handling the error if 
you do not catch an error. 
The ability to catch an error can 
be very helpful if there is an issue 
on a live website. 
It lets you tell users that 
something has gone wrong 
(rather than not informing them 
why the site stopped working).

--------

**FINALLY** 
The contents of the fi na 11 y 
code block will run either 
way - whether the try block 
succeeded or failed. 
It even runs if a return keyword 
is used in the try or catch block. 
It is sometimes used to clean up 
after the previous two clauses. 
These methods are similar 
to the .done(), . fail(), and 
. a 1 ways() methods in jQuery. 
You can nest checks inside each 
other (place another t ry inside a 
catch), but be aware that it can 
affect performance of a script.

----------

**THROWING ERRORS**
If you know something might cause a problem for your script, you can 
generate your own errors before the interpreter creates them.

----------

**THROW ERROR FOR NaN**
If you try to use a string in a 
mathematical operation (other 
than in addition), you do not get 
an error, you get a special value 
called NaN (not a number). 
 
In this example, a try block 
attempts to calculate the area of 
a rectangle. If it is given numbers 
to work with. the code will run.

If it does not get numbers, a 
custom error is thrown and the 
catch block displays the error.

By checking that the results 
are numeric, the script can fail 
at a specific point and you can 
provide a detailed error about 
what caused the problem (rather 
than letting it cause a problem 
later in the script).

--------

## COMMON ERRORS 
Here is a list of common errors you might find 
with your scripts.
* GO BACK TO BASICS
* MISSED/ EXTRA CHARACTERS 
* DATA TYPE ISSUES 

--------

* If you understand execution contexts (which have two 
stages) and stacks, you are more likely to find the error 
in your code. 

* Debugging is the process of finding errors. It involves a 
process of deduction. 

* The console helps narrow down the area in which the 
error is located, so you can try to find the exact error. 

* JavaScript has 7 different types of errors. Each creates 
its own error object, which can tell you its line number 
and gives a description of the error. 

* If you know that you may get an error, you can handle 
it gracefully using the try, catch, finally statements. 
Use them to give your users helpful feedback. 





















































































