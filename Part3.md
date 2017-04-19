## Part 3

### Quick Part 2 Review
Remember that triangles can be made with a CSS border trick, and the transform property can rotate things:
```
.triangle {
  width: 0;
  height: 0;
  border-top: 50px solid blue;
  border-right: 50px solid green;
  border-bottom: 50px solid yellow;
  border-left: 50px solid red;
}
.diamond {
  transform: rotate(45deg);
  width: 100px;
  height: 100px;
  background-color: blue;
}
```

### Creating Animations!
CSS animations make an HTML element change from one set of CSS styles to another set.

Each set of css is called a _keyframe_. Here is an example of defining keyframes in CSS:
```
@keyframes color-change {
    from {
      background-color: red;
    }
    to {
      background-color: yellow;
    }
}
```
There are several things to notice.
- This is the only time in CSS when you have a set of curly braces inside a set of curly braces! Keep curly braces organized.
- In this case, the two keyframes are `from` and `to`, meaning that the HTML element that uses this animation will go _from_ red _to_ yellow.
- In the first line, `@keyframes color-change`, color-change can be anything.

After defining a set of keyframes, nothing will happen yet, because somewhere else in the CSS needs to actually use the animation.

```
.square {
    width: 100px;
    height: 100px;
    background-color: blue;
    
    animation-name: color-change;
    animation-duration: 4s;
}
```
Notice where it says `animation-name: color-change`. That's how the web browser knows which set of keyframes to use!

The next line, `animation-duration: 4s`, means that the animation will last 4 seconds. Notice how the square takes 4 seconds to change from red to yellow.

After four seconds though, the square is blue. Why? Because `background-color: blue` is in the CSS for `.square`! To make animations repeat infinitely, add this line:
```
animation-iteration-count: infinite;
```
Remember, anything can be changed, not just color. For example, these keyframes would move the square across the screen while changing its color in 5 seconds:
```
@keyframes move {
    from {
      left: 0;
      background-color: red;
    }
    to {
      left: 400px;
      background-color: blue;
    }
}
.moving-square {
  position: absolute;
  left: 0;
  width: 100px;
  height: 100px;
  background-color: blue;
  animation-name: move;
  animation-duration: 5s;
}
```
Just think about how the div should start out looking like, and then end up looking like.


#### Multiple Keyframes
Feeling adventurous? Try figuring out what this does:
```
@keyframes many-color-changes {
    0%   {background-color: red;}
    25%  {background-color: yellow;}
    50%  {background-color: blue;}
    100% {background-color: green;}
}
```


### Challenges




