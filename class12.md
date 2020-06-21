# Basic usage of canvas

```javascript

<canvas id="tutorial" width="150" height="150"></canvas>

```

***NOTE :the canvas will initially be 300 pixels wide and 150 pixels high if no specified attributs added***

- you can style `canvas` using css properties just like the images
- you should provide fallback content to be displayed by older browsers.


To display something in the canvas , a script first needs to access the rendering context and draw on it. The `<canvas>` element has a method called getContext(), used to obtain the rendering context and its drawing functions.

```javascript

var canvas = document.getElementById('tutorial');
var ctx = canvas.getContext('2d');

```

# Drawing shapes with canvas

- The grid : The origin of the grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). 

- `<canvas>` only supports two primitive shapes: rectangles and paths (lists of points connected by lines) All other shapes must be created by combining one or more paths

- There are three functions that draw rectangles on the canvas:
  - fillRect(x, y, width, height) : Draws a filled rectangle.
  - strokeRect(x, y, width, height) : Draws a rectangular outline.
  - clearRect(x, y, width, height) : Clears the specified rectangular area, making it fully transparent.
```javascript

  function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}

```
# Drawing paths

- First, you create the path. `beginPath()`
- use drawing commands to draw into the path. `moveTo` `lineTo`
- stroke or fill the path to render it. `stroke()` `fill()`

# Applying styles and colors

- fillStyle : Sets the style used when filling shapes.
```javascript

function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  for (var i = 0; i < 6; i++) {
    for (var j = 0; j < 6; j++) {
      ctx.fillStyle = 'rgb(' + Math.floor(255 - 42.5 * i) + ', ' +
                       Math.floor(255 - 42.5 * j) + ', 0)';
      ctx.fillRect(j * 25, i * 25, 25, 25);
    }
  }
}

```
- strokeStyle : Sets the style for shapes' outlines.

```javascript

function draw() {
    var ctx = document.getElementById('canvas').getContext('2d');
    for (var i = 0; i < 6; i++) {
      for (var j = 0; j < 6; j++) {
        ctx.strokeStyle = 'rgb(0, ' + Math.floor(255 - 42.5 * i) + ', ' + 
                         Math.floor(255 - 42.5 * j) + ')';
        ctx.beginPath();
        ctx.arc(12.5 + j * 25, 12.5 + i * 25, 10, 0, Math.PI * 2, true);
        ctx.stroke();
      }
    }
  }
  ```

  # Drawing text

- fillText(text, x, y [, maxWidth]) :Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- strokeText(text, x, y [, maxWidth]) :Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

# Styling text

- font = value :The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
- textAlign = value : Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
- textBaseline = value :Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
- direction = value :Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.
