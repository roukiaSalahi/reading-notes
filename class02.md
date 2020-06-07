# HTML

## Text

When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.

tags  |  purpose
---------------|--------------------------------------------------------------------
`<h1>..<h6>`   | used for heaading 
`<p>`          |  to create a paragraph
`<b> `         | to make characters appear bold.
`<i>`          | to make characters appear italic
`<sup>`        | raising number to a power
`<sub> `       | foot notes or chemical formula
`<br />`       | add a line break inside the middle of a paragraph
`<hr /> `      | To create a break between themes
`<strong> `    | indicates that its content has strong importance
`<em> `        | indicates emphasis that subtly changes the meaning of a sentence
`<blockquote>` | used for longer quotes that take up an entire paragraph
`<q>`          | used for shorter quotes that sit within a paragraph


# CSS

## Introduction

CSS allows you to create rules that specify how the content of an element should appear. it works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration. declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon

If there are two or more rules that apply to the same element, it is important to understand which will take precedence.

- LaSt ruLe : If the two selectors are identical, the latter of the two will take precedence
- SpecIfIcIty : If one selector is more specific than the others, the more specific rule will take precedence over more general ones. In this 
- IMportant : You can add !important after any property value to indicate that it should be considered more important than other rules that apply to the same element

***Note : its better to use external link for css because all of your web pages can share the same style sheet and the same code does not need to be repeated in every page also the site will load faster.***

```javascript

<link href="css/styles.css" type="text/css" rel="stylesheet" />

```

# JavaScript

## Basic javaScript instructions

### Statments

Each individual instruction or step is known as a statement. Statements should end with a semicolon. 

### Code blocks 

used to group together many more statements. This helps programmers organize their code and makes it more readable. 

### Coments in JavaScript

```javascript
/* comment goes here for multi line */

// comment goes here for single line

```
### What is a variable ?

A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables. The data stored in a variable can change (or vary) each time a script runs. 

### How to declare and assign variables ?

```javascript
var quantity ;
quantity = 3 ;

```
***Note : if a variable name is more than one word, it is usually written in camelCase***

### Data type

Data type  |  purpose
-----------|--------------------------------------------------
Numbers    |  counting, calculations sums, size, amount of time 
String     |  add new content into a page
Boolean    |  determining which part of script should run

***example to store a number :***

```javascript

var price , quantity , total; 
price = 5; 
quantity = 14; 
total = price * quantity; 

```

***example to store a string :***


```javascript

var username , message; 
username = 'Molly'; 
message = 'See our upcoming range';  

```
***Notes : string must always be written surrownded with double or single quotes and should always be in one line***

-[x] "helo" or 'helo'
-[ ] 'helo" or "helo'

***example to store a boolean :***

```javascript

var i nStock , shipping; 
inStock = true; 
shipping= false; 

```
***Note : booleans are used when your code can take more than one path. diffrent code may run in diffrent circumstances.***

### Rules for naming variables

-[x] must begin with `letter`, `$`,`_`
-[ ] must not start with a number

-[x] can contain `letter`,`numbers`, `$`,`_`
-[ ] must not contain `-`, `.`

-[x] describe the kind of information
-[ ] cant be a keyword

### Arrays :

it is a special type of variables, it doesnt just store one value it stores a list of values. you use arrays whenever you are working with a list or a set of values that are related to each other and when you do not know how many items a list will contain because, when you create the array, you do not need to specify how many values it will hold. 

example of creating, accessing, changing values in an array:

```javascript

// Create the array
var colors = ['white', 'black' , 'custom']; 
// Update the third item in the array
colors[2] = 'beige' ; 
// Get the element with an id of colors
var el = document.getElementByid(' colors') ; 
// Replace with third item from the array
el.textContent = colors[2];

```

## Decisions and loops

### flowchart

there are often several places in a script where decisions are made that determine which lines of code should be run next. flowcharts can help you plan for these occasions.

Evaluation of a condition in order to make a decision, your code checks the current status of the script. this is commonly done by comparing two values using a comparision operator which returns a value of true or false.

conditional statement is based on a concept of if/then/else; if a condition is met then your code executes one or more statements, else your code does something different or just skip the step.

![if statment flowchart](https://2.bp.blogspot.com/-YimkS2x7vyA/T3tLwSL3TYI/AAAAAAAAAGY/9Wct8reM2VU/s1600/if.jpg)























### How to assign variables ?