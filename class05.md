# HTML

## images

`<img>`: its an empty element which mean you dont have to add a closing tag .it must carry the following two attributes:
- src : This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. 
- alt : This provides a text description of the image which describes the image if you cannot see it.
- title :to provide additional information about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image.

***Note : Images often take longer to load than the HTML code that makes up the rest of the page. It is, therefore, a good idea to specify the size of the image so that the browser can render the rest of the text on the page while leaving the right amount of space for the image that is still loading.***


```javascript
<img src="images/quokka.jpg" alt="A family of quokka" width="600" height="450" /> 

```

### rules for CreatIng Image:
1. save images in the rIght format : jpeg, gif, or png format
2. save images at the rIght size : You should save the image at the same width and height it will appear on the website. 
3. use the correCt resolutIon :  saving images at a higher resolution results in images that are larger than necessary and take longer to download.

# CSS

## Colors

### Foreground color

The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways

- rgb values : stand for red, green and blue

```javascript

p { 
    color: rgb(100,100,90);
    }

```

- hex Codes :

```javascript

p { 
    color: #ee3e80;
    } 

```

- Color names :

```javascript

p { 
    color: DarkCyan;
    } 

```

### background colors

same as color but you can specify the background color for that element
```javascript

body { 
    background-color: rgb(200,200,200);} 
h1 { 
    background-color: DarkCyan;} 
h2 { 
    background-color: #ee3e80;} 
p { 
    background-color: white;} 

```
***Note: By default, most browser windows have a white background, but browser users can set a background color for their windows, so if you want to be sure that the background is white  you can use the background-color property on the `<body>` element.***

### Color picker tool 

Color picking tools are available in image editing programs like Photoshop and GIMP. You can see the RGB values specified next to the radio buttons that say R, G, B.
The hex value is provided next to the pound or hash # symbols

## Text 

Typeface  | properites
------------|-------------------------------------------------------------------------
serif       |  have extra details on the end of the main strokes of the letters.
sans-serif  |  have straight ends to letters, and therefore have a much cleaner design
monospace   |  every letter in a monospace (or fixed-width) font is the same width.

***Note : When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.***
***Note : you can add any type of font you want by installing from google in your computer or by adding the link of the font to you css file***

text properties | purpose
-------------------|----------------------------------------------------------------------
`font-family`      | to change the size of the text
`font size`        | to change the type of the familt
`font-weight`      | to specify the wight of the text either bold or normal
`font-style`       | to specify the style of the text either normal or italic of oblique
`text-decoration`  | to add or remove lines under or over the text 




