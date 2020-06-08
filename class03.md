# HTML

## Lists


tag   | meaning
---------|-------------------
`<ol>`   |  ordered list 
`<ul>`   |  unordered list 
`<dl>`   |  definition list 
`<dt>`   |  definition term 
`<dd> `  |  definition


# CSS

## Boxes

### box dimensions

By default a box is sized just big enough to hold its contents. To set an dimensions for a box you can use the height and width properties.


### Limmiting width and height

- min-width/height property specifies the smallest size a box can be displayed at when the browser window is narrow

- max-width/height property indicates the maximum width a box can stretch to when the browser window is wide.

```javascript

p { 
    min-height: 10px;
    max-height: 30px;
    min-width: 450px;
    max-width: 650px; }

```


### overflow

The overflow property tells the browser what to do if the content contained within a box is larger than the box itself

- hidden This property simply hides any extra content that does not fit in the box.
- scroll This property adds a scrollbar to the box so that users can scroll to see the missing content

```javascript

p.one { 
    overflow: hidden;}
p.two { 
    overflow: scroll;}

```

### Border, margin and Padding

- Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.
- Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
- Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents. 

***Note : If you specify a width for a box, then the borders, margin, and padding are added to its width and height***

### border-width

The border-width property is used to control the width of a border. The value of this property can be used thin, medium or thick

### border-style  

style    | display
------------|-----------------------------------------------
solid       | a single solid line
dotted      | a series of square dots 
dashed      | a series of short lines
double      | two solid lines 
groove      | appears to be carved into the page
ridge       | appears to stick out from the page
inset       | appears embedded into the page
outset      | looks like it is coming out of the screen
hidden/none | no border is shown

# JavaScript

## Decisions and Loops

### Switch statment

A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value

***Note: At the end of each case is the break keyword. It tells the JavaScript interpreter that it has finished with this switch statement and to proceed to run any subsequent code that appears after it.***

### if vs switch statments

if :

- There is no need to provide an else option. (You can just use an if statement.) 
- With a series of if statements, they are all checked even if a match has been found (so it performs more slowly than switch). 

switch :

- You have a default option that is run if none of the cases match. 
- If a match is found, that code is run; then the break statement stops the rest of the switch statement running (providing better performance than multiple i f statements.

### type correction 

when JavaScript convert data types behind the scenes to complete an operation

### weak typing 

the data type for a value can change. Some other languages require that you specify what data type each variable will be. They are said to use strong typing

***Note : NaN is a value that is counted as a number. You may see it when a number is expected, but is not returned, e.g .. ('ten' /2) results in NaN.***

### loops

loops check a condition. if it returns true, a code block will run. then the condition will be checked again if it still return true, the code block will run again. it repeats until the condition returns false. 

#### types of loops

- for : to run the code specific number of times, the condition is usually a counter which indicate how many time the loop should run.
- while : if you dont know how many times the code should run, the code will countinue to loop for as long as the condition is true.
- do while : it will alwayes run the statments inside the curly braces at least onece even if the condition is false.

***Nots :*** 
- ***Any variable you can define outside of the loop and that does not change within the loop should be defined outside of it. If it were declared inside the loop, it would be recalculated every time the loop ran, needlessly using resources.***
- ***break This keyword causes the termination of the loop and tells the interpreter to go onto the next statement of code outside of the loop. (You may also see it used in functions.)***
- ***continue This keyword tells the interpreter to continue with the current iteration, and then check the condition again. (If it is true, the code runs again.)***

Examples of using for loops :

```javascript

var scores= [24. 32, 17];             //Array of scores
var arraylength scores.length;       // Items in array
var roundNumber = O;                //Current round 
var msg '';                        //Message 
var i ;                           // Counter 
//Loop through the items in the array 
for (i = O; i < arraylength; i++) { 
//Arrays are zero based (so 0 is round 1) 
//Add 1 to the current round 
roundNumber = (i + l); 
// Write the current round to message 
msg += 'Round ' + roundNumber + ' : '; 
//Get the score from the scores array 
msg += scores[i] + '<br / >' ; 
}
document.getElementByid( 'answer') .innerHTML msg; 

```
Example of using do while loops

```javascript

var i = l ; //Set counter to 1 
var msg = ' ' ;  // Message
 
//Store 5 times table in a variable 
do { 
msg += i + ' x 5 = ' + (i * 5) + '<br I>' ;s i++; 
 } wh il e ( i < 1) ; 
//Note how this is already 1 and it still runs 
document.getEl ementByid( ' answer') . innerHTML = msg; 

```

