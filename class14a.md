# CSS

## transform

CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

values      | purpose
------------|--------------------------------------------------------------------------------------------------------------------
rotate      |  rotate an element from 0 to 360 degrees
scale       |  change the appeared size of an element
scaleX      |  scale the width of an element
scaleY      |  scale the height of an element
translate   |  pushing and pulling an element in different directions without interrupting the normal flow of the document
translateX  |  change the position of an element on the horizontal axis 
translateY  |  change the position of an element on the vertical axis
skew        |  distort elements on both the horizontal axis and vertical axis
skewX       |  distorts an element on the horizontal axis
skewY       |  distorts an element on the vertical axis
rotate      | +values will rotate the element around its dedicated axis clockwise, while -values will rotate the element counterclockwise.


***NOTE : The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.***

***NOTE : +values >> rotation clockwise and -values >> rotation counterclockwise***

### Combining Transforms

```javascript

.box-1 {
  transform: rotate(25deg) scale(.75);
}
.box-2 {
  transform: skew(10deg, 20deg) translateX(20px);
}

```


***NOTE : Using multiple transform declarations will not work, as each declaration will overwrite the one above it***

## Perspective

In order for three-dimensional transforms to work the elements need a perspective from which to transform. The perspective for each element can be thought of as a vanishing point, similar to that which can be seen in three-dimensional drawings.

- using the perspective value within the transform property on individual elements
- using the perspective property on the parent element residing over child elements being transformed.

values      | purpose
---------------------|--------------------------------------------------------------------------------------------------------------------
none                 |  turns off any perspective
length measurement   |  set the depth of the perspective


### 3D Rotate

```javascript

.box-1 {
  transform: perspective(200px) rotateX(45deg);
}
.box-2 {
  transform: perspective(200px) rotateY(45deg);
}
.box-3 {
  transform: perspective(200px) rotateZ(45deg);
}

```



### 3D Scale

```javascript

.box-1 {
  transform: perspective(200px) scaleZ(1.75) rotateX(45deg);
}
.box-2 {
  transform: perspective(200px) scaleZ(.25) rotateX(45deg);
}

```

### 3D Translate

```javascript

.box-1 {
  transform: perspective(200px) translateZ(-50px);
}
.box-2 {
  transform: perspective(200px) translateZ(50px);
}

```
## Transitions
for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.
There are four transition related properties :
- ransition-property
- transition-duration
- transition-timing-function
- transition-delay

```javascript

.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}

```

```javascript

.box {
    background: #2db34a;
    border-radius: 6px
    transition-property: background, border-radius;
    transition-duration: 1s;
    transition-timing-function: linear;
  }
  .box:hover {
    background: #ff7b29;
    border-radius: 50%;
  }

  ```




