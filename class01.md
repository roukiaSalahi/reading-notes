# HTML

## What are Elements and attributes ?

HTML uses elements to describe the structure of pages, however attributes provide additional information about the contents of an element.

### id & class atrributes

These attribute used to uniquely identify elements.

id attribute identify one element from other elements, however class attribute identify several elements as being different from the other elements on the page.

***Note : If you would like to indicate that an element belongs to several classes, you can separate class names with a space.***

```javascript

<p id="pullquote"> paragraph goes here </p>

<p class="important"> paragraph goes here </p>

<p class="important admittance"> paragraph goes here </p>

```

### div & span elements

we use `<div>` to group a set of elements together in one block-level box.

we use `<span>` to Contain a section of text or  inline elements.

***Note : you can create CSS style rules to indicate how the appearance of all the elements contained within.***

```javascript

<div id="header">
....

</div>

<p> paragraph goes here <span class="gallery">section of text  goes here </span> continue the paragraph </p>

```

### iframe

is like a little window so you can see another page

```javascript

<iframe
width="450" height="350"src="">
</iframe>

```

### meta

The `<meta>` element lives inside the`<head> `element so its not visible to users but it contains information about that web page such as the decribtion of the page, autor name, keywords, expires date ,and many features.


## How to Comment in html

comments are not visible to user's browser its only visible in the source code. We use comments to make our code much easier to understand.

```javascript
<!-- comment goes here -->

```

## HTML5 LAYOUT

Traditional HTML layouts web page authors used `<div>` elements to group together related elements on the page and used class or id attributes to indicate the role of the `<div>` element in the structure of the page, however the new html layout elements allow you to divide up the parts of page with elements that name indicate the kind of content you will find in them  in order to help describe the structure of the page and make the code easier to follow.

html5 layout elements    |  purpose/content
---------------|------------------------------------------------------------------------------
`<header>`     |  site name and main navigation
`<footer>`     |  copyright,links privacy policy 
`<nav>`        |  primary site navigation
`<article>`    |  independent piece of content
`<aside>`      |  content related to entire page or not essential info inside article 
`<section>`    |  diffrent sections of the page 
`<hgroup>`     |  group set of one or more `<h1>...<h6>` 
`<figure>`     |  any content that is referenced from main flow of article
`<div>`        |  group set of elements when there is no suitable one

***Note: you should include in css which elements should be rendered as a block-level elements as the following example***

```javascript

header, section, footer, aside, nav, article, figure {
    display: block;
}

```

# JavaScript

## How javascript makes web pages more interactive ?

1. Access content
2. Modify content 
3. Program rules 
4. React to event 

## What is a script ?

script is a series of instructions that a computer can follow to achive goal. scripts can run diffrent section of the code in response to the situation around them and the browser may use diffrent parts of the script depending on how the user interacts with the page.

## How do computers fit with the world around them ?

computers create models of the world using data, so the browser recive a page as html code then create a model of the page and store it in the memory after that it use a rendering engine to show the page on screen.

the model use objects to represent physical things, objects can have properties that tell us about the object, methods that perform tasks using the properties of that object, events which are triggered when a user interact with computer, so they all fit togather events can trigger methods and methods can retrieve or update an object properties.

*example :*

document object : represent the whole document 
 propereties : such as the title of the page.

 method : is like getting information from spesific element or adding new content.

 event : happen when the user clicking or tapping on an element.



