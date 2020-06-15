# HTML

## Tables

tag         |  purpose
------------|----------------------------------------------------------------------------------
`<table>`   | used to create a table.
`<tr>`      | indicate the start of each row stands for table row.
`<td>`      | cell of a table stands for table data.
`<th>`      | epresent the heading for either a column or a row stands for table heading
`<thead>`   | The headings of the table should sit inside the this element
`<tbody>`   | The body should sit inside the this element. 
`<tfoot>`   | The footer belongs inside the this element.

# JavaScript


### CREATING OBJECTS USING LITERAL NOTATION

```javascript

var hotel = {} 
hotel .name= 'Quay'; 
hotel .rooms = 40;
hotel.booked = 25;
hotel.checkAvailabil ity =function() {
  return this.rooms - this.booked; 
};

```

```javascript

var hotel = { 
    name: 'Quay' , 
    rooms: 40, 
    booked: 25, 
    checkAvailability: function() { 
        return this.rooms - this.booked; 
    } 
}; 

```

### CREATING OBJECTS USING CONSTRUCTOR SYNTAX 

```javascript

var hotel = new Object(); 
hotel.name= 'Park'; 
hotel.rooms = 120; 
hotel .booked = 77; 
hotel .checkAvailability = function() {
return this.rooms - this.booked;
};

```
- to create multiple objects

```javascript

function Hotel(name, rooms, booked) { 
    this.name = name; 
    this.rooms = rooms; 
    this.booked = booked; 
    this.checkAvailability = function() 
    return this.rooms - this.booked; 
    } ; 
var quayHotel =new Hotel('Quay', 40, 25); 
var parkHotel =new Hotel('Park', 120, 77); 

```

***Note : this keyword is used instead of the object name to indicate that the property or method belongs to the object that this function creates***

### ARRAYS IN AN OBJECT 
 the property of any object can hold an array

### OBJECT IN AN ARRAY
the value of any element in an array can be an object

### WHAT ARE BUILT-IN OBJECTS

Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages. As soon as a web page has loaded into the browser, these objects are available to use in your scripts. You access their properties or methods using dot notation, just like you would access the properties or methods of an object you had written yourself

- BROWSER OBJECT MODEL 
The Browser Object Model contains objects that represent the current browser window or tab. It contains objects that model things like browser history and the device's screen. 

- DOCUMENT OBJECT MODEL 
The Document Object Model uses objects to create a representation of the current page. It creates a new object for each element (and each individual section of text) within the page. 

- GLOBAL JAVASCRIPT OBJECTS 
The global JavaScript objects represent things that the JavaScript language needs to create a model of. For example, there is an object that deals only with dates and times



