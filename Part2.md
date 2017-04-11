## Part 2

### Quick Part 1 Review
Remember that divs are just boxes in HTML, and that classes can be used to apply different CSS to certain HTML elements, depending on which class is specified. Also, multiple classes can be used. Be able to understand this example:
```
.blue {
  background-color: blue;
}
.red {
  background-color: red;
}
.square {
  width: 100px;
  height: 100px;
}
```
```
<div class="square blue"></div>
<div class="square red"></div>
```

### Triangles
There is no official triangle HTML element, but there is a CSS trick to make a triangle. Try this:
```
.triangle {
  width: 0;
  height: 0;
  border-top: 50px solid blue;
  border-right: 50px solid green;
  border-bottom: 50px solid yellow;
  border-left: 50px solid red;
}
```
To just have a single triangle, change the color to `transparent` for the borders you don't need.


### CSS box-shadow
This page explains box-shadows pretty well: <https://css-tricks.com/almanac/properties/b/box-shadow/>


### CSS transform
The CSS `transform` property has several functions. One usecase is for rotation. For example:
```
.diamond {
  transform: rotate(45deg);
  width: 100px;
  height: 100px;
  background-color: blue;
}
```


### Challenges
Try making the following things by combining shapes:
- heart (two circles and a rotated square)
- Pacman (a circle and a triangle, and more circles for its food)
- speech bubbles
- magnifying glass
- house (add windows and a door too!)
- smartphone





