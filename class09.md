# HTML 

## Forms

There are several types of form controls that you can use to collect information from visitors to your site.

- Password input: Like a single line text box but it masks the characters entered.
- Text input (single-line) : Used for a single line of text such as email addresses and names.
- Text area (multi-line) : For longer areas of text, such as messages and comments
- Checkboxes : When a user can select and unselect one or more options.
- Radio buttons : For use when a user must select one of a number of options.
- Drop-down boxes : When a user must pick one of a number of options from a list
- Image buttons : Similar to submit buttons but they allow you to use an image.
- Submit buttons : To submit data from your form to another web page.
- File upload : Allows users to upload files (e.g. images) to a website.

```javascript

<form action="http://www.example.com/login.php"> 
<p>Username:  
<input type="text" name="username" size="15"    maxlength="30" /> 
</p> 
</form>

```

```javascript

<form action="http://www.example.com/profile.php"> 
<p>Please select your favorite music service(s):  <br />   
<input type="checkbox" name="service" value="itunes" checked="checked" /> iTunes   
<input type="checkbox" name="service" value="lastfm" /> Last.fm   
<input type="checkbox" name="service" value="spotify" /> Spotify 
</p> 
</form> 

```

```javascript

<form action="http://www.example.com/profile.php"> 
 <p>What device do you listen to music on?
 </p> 
 <select name="devices">    
 <option value="ipod">iPod</option>    
 <option value="radio">Radio</option>   
 <option value="computer">Computer</option>  
 </select> 
 </form> 

 ```

# CSS

## Lists: 

property | purpose
----------------------|--------------------------------------------------------------------------------------------
`list-style-type`     | control the shape or style of a bullet point
`list-style-image`    |  specify an image to act as a bullet point
`list-style-position` | indicates whether the marker should appear on the inside/outside
`list-style`          | allows you to express the markers' style, image and position properties in any order

## Tables

property | purpose
----------------------|------------------------------------------------------------------------
`width`               | set the width of the table
`padding`             | set the space between the border of each table cell and its content
`text-transform`      | convert the content of the table headers to uppercase
`letter-spacing`      | add additional styling to the content of the table headers
`border-top/bottom `  | set borders above and below the table headers
`text-align`          | align the writing of table cells 
`:hover`              | highlight a table row when a user's mouse goes over it
`empty-cells`         | specify whether or not their borders should be shown.
`border-spacing`      |control the distance between adjacent cells
` border-collapse`    |Borders are collapsed into a single border where possible

## Forms

property | purpose
----------------------|--------------------------------------------------------------------------------------
`font-size`           |  sets the size of the text entered by the user.
`color`               |  sets the text color
`background-color `   |  sets the background color of the input
`border`              |  adds a border around the edge of the input box
`border-radius `      |  can be used to create rounded corners
` :focus `            |  change the background color of the text input when it is being used,
`:hover`              |  applies the same styles when the user hovers over them
`background-image `   |  background-image 
`text-shadow `        |  give a 3D look to the text in browsers that support this property.
` border-bottom `     |  make the bottom border of the button slightly thicker,
`cursor`              | allows you to control the type of mouse cursor that should be displayed to users.















