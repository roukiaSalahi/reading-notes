# CSS

## Layout

CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box

- Block-level boxes : start on a new line and act as the main building blocks of any layout.
  - Block-level elements start on a new line Examples include: `<h1> <p> <ul> <li>`
  - If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.


- inline boxes : flow between surrounding text. 
  - inline elements flow in Between surrounding text Examples include: `<img> <b> <i>`


***Note : You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors***

### containing ElEmEnts

tag | purpose 
--------|-------------------------------------------------------------------------------------------------------------------
z-index | to control which element sits on top
float   | to take an element in normal flow and place it as far to the left or right of the containing element as possible.
clear   |  no element (within the same containing element) should touch the left or righthand sides of a box

### relative positioning 

```javascript
p.example { 
    position: relative; 
    top: 10px; left: 100px;
}
```

### absolute positioning

```javascript

h1 { 
    position: absolute; 
    top: 0px; left: 500px; width: 250px;
    } 

```

### Screen sizes

Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).

### fixed width Layouts

do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.
Liquid Layouts|stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.

### Css frameworKs

- advantages
  - They save you from  
  - repeatedly writing code for the same tasks.
  - They will have been tested across different browser versions (which helps avoid browser bugs).

- disadvantages
  - They often require that you use class names in your HTML code that only control the presentation of the page (rather than describe its content
  - in order to satisfy a wide variety of needs, they often contain more code than you need for your particular web page (commonly referred to as code “bloat”).






