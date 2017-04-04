# CSS Art Workshop

#### Inspiration
This workshop was inspired by [A Single Div](http://a.singlediv.com/). Check out the site - everything on that page is made purely out of HTML/CSS, no images at all!

#### Goals
Although realistically most websites don't draw pictures with code, this workshop is a good exercise to learn more about CSS. In the process of making their drawings, participants will learn about the following:
- changing size and color
- creating different shapes (rectangles, rounded rectangles, circles, triangles)
- positioning shapes
- animation

#### Target Audience
Participants should already have basic experience with HTML and CSS. Ideally, participants should be familiar with:
- Divs
- Classes and IDs

#### Setup
- Use [JSBin](http://jsbin.com), an online HTML/CSS editor. (Similar alternatives include [CodePen](http://codepen.io) & [JSFiddle](http://jsfiddle.net)
  - Make an account to save work!

## Part 1

### Quick HTML & CSS Review

#### HTML Divs

#### CSS Basics

#### Classes and IDS

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
