## Part 1

### Quick HTML & CSS Review

#### HTML Divs
```
<div></div>
```
A div is an HTML element that is like a general purpose box. It is probably the most commonly used tag.

#### CSS Basics
```
div {
  width: 100px;
  height: 100px;
  background-color: blue;
}
```
CSS always refers to an HTML element, and defines how the HTML element should look. In this example, all `div`s will be blue and have a width and height of 100 pixels.

#### Classes and IDS
Not every single div should be blue, though. This where classes (think _class_ification) and IDs (used to _id_entify a single element) come into play. First remember the difference between the two:
- Classes create _classifications_ for HTML elements
  - for example, a bunch of divs could have the class `blue-box` and a few others could have the class `red-box`
- IDs _identify_ a single HTML element
  - for example, only one HTML element can have the `special-box` id

For a full example:
```
<div class="blue-box"></div>
<div class="blue-box"></div>

<div id="special-box"></div>
```
```
.blue-box {
  background: blue;
}
#special-box {
  background: purple;
}
```
For this workshop, everything will be done with divs and classes.


### Size and Color
```
.blue-square {
  width: 200px;
  height: 200px;
  background: blue;
}
```
- Use a [color picker](https://www.google.com/search?q=color+picker) to pick your own colors
- px = pixels
- 100px is approximately 1 inch

### Rounded Corners
```
.rounded-square {
  width: 200px;
  height: 200px;
  background: blue;
  
  border-radius: 20px;
}
```
### Making a Circle
- If you make the `border-radius` _at least half_ of what the width and height are, the div becomes a circle!
  - for example - if the width and height is 200px, the border-radius needs to be 100px (half of 200)
```
.circle {
  width: 200px;
  height: 200px;
  background: blue;
  
  border-radius: 100px;
}
```

### Positioning
- First set `position: absolute;` 
- Then set `top: 200px;` and `left: 100px;`
  - `top` is how many pixels from the top edge of the screen
  - `left` is how many pixels from the left edge of the screen

```
.blue-square {
  width: 200px;
  height: 200px;
  background: blue;
  
  position: absolute;
  top: 100px;
  left: 100px;
}
```

### New concept: Multiple classes for a single div
HTML elements can have _multiple classes_, just separated by a space. For example:
```
<div class="blue-square"></div>
<div class="blue-square rounded"></div>
```
```
.blue-square {
  width: 200px;
  height: 200px;
  background: blue;
}
.rounded {
  border-radius: 20px;
}
```
The first div will be a blue square, and the second div will be a blue square with rounded corners.

## Part 1 Challenge
If you [Google "Mondrian art"](https://www.google.com/search?q=mondrian+art&tbm=isch), you'll see images like this:

![Mondrian art](https://s-media-cache-ak0.pinimg.com/originals/ba/20/d7/ba20d7c9a9db61be00e80cd84f3f0e3c.jpg)

Make your own, using divs, positioning, and mulitple classes!
