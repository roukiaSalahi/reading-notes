# HTML

## links

`<a>` : Links are created using the <a> element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.

- mailto: To create a link that starts up the user's email program and addresses an email to a specified email address, 

```javascript

<a href="mailto:jon@example.org">Email Jon</a> 

```
### linking to a specifec part of the same page

 you use the `<a>` element again, but the value of the href attribute starts with the # symbol, followed by the value of the id attribute of the element you want to link to

 ```javascript

<a href="#arc_shot">Arc Shot</a><br /> 

```

### linking to a specific part of another page

As long as the page you are linking to has id attributes that identify specific parts of the page, you can simply add the same syntax to the end of the link for that page.
Therefore, the href attribute will contain the address for the page (either an absolute URL or a relative URL), followed by the  # symbol, followed by the value of the id attribute that is used on the element you are linking to

```javascript

<a href="http:/www. htmlandcssbookcom/ #bottom">

```

# CSS

## Layout

### ControLLing the position of eLements

- normal flow : Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else).

- relative positioning :This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.

```javascript

p.example{ 
    position: relative;
    top: 10px;
    left: 100px;
  }

```

- absolute positioning :This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.

```javascript

h1 { 
    position: absolute;
    top: 0px; left: 500px; width: 250px;
    }
p { 
    width: 450px;
    }

```

### Floating elements

allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.you can also use float to place elements side by side


### box offset

 to tell the browser how far from the top or bottom and left or right it should be placed

 
# JavaScript

## Functions

Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements). The function acts like a store; it holds the statements that are contained in the curly braces until you are ready to use them. Those statements are not run until the function is called
 
 ### How to declare a function 

 create a function you give it a name then write the statements needed to achive its task inside the curly braces. to run the code in the function you use the function name followed by parantheses. sometimes a function needs specific information to perform its task in such cases when you declare the function you give it parameters inside the fuction that acts like variables,  you can call the function as many times as you want

### How to call a function 

when you call a function that has parameters you specify the values it should use in the parenthess that follwo its name the values are called arguments and they can be provided as values or as variables

example:


```javascript

function getSize(width, height, depth) { var area = width * height; 
} 
var volume = width * height * depth; var sizes= [area, volume]; return sizes; 
var areaOne = getSize(3, 2, 3)[0]; var volumeOne = getSize(3, 2, 3)[1]; 

```


### Local variables

When a variable is created inside a function using the var keyword, it can only be used in that function.

- If the function runs twice, the variable can have different values each time. 
- Two different functions can use variables with the same name without any kind of naming conflict


### Global variables

If you create a variable outside of a function, then it can be used anywhere within the script. It is called a global variable and has global scope

***Note : Each variable that you declare takes up memory. The more variables a browser has to remember, the more memory your script requires to run. Scripts that require a lot of memory can perform slower, which in turn makes your web page take longer to respond to the user.***