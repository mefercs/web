# Applied Visual Design

- Opacity: 0 - 1
Visualize the hit boxes.
```html
*{
    box-sizing:border-box;
    outline:1px solid limegreen !important
  }
```

#### Text Align property

|`text-align`| description|
|---|---|
|justify|Spaces the text, each line has equal width|
|center|Centers the text|
|right|right-aligns the text|
|left|(is the default)left aligns the text|

- `font-weight: bold` to create a strong tag or you can use the `<strong></strong>` tag. Or we can use a value (200,300,400 ...)
- `text-decoration: undeline/line-through` to undeline, or you can use the `<u></u> / <s></s>` tag.
- `font-style: italic` or us the `<em></em>` tag.
- `font-size: value`
- `text-transform: value` where value = lowercase/uppercase/capitalize/initial/inherit/none
- `<hr>` an horizontal line.
- `rgba()` where a means  alpha/level of opacity
- `line-height` or the space between the text lines

#### BOX SHADOW

|box-shadow|offset-x|offset-y|blur-radius|spread-radius|color|
|---|---|---|---|---|---| 
|Description|x offset(px)|y offset(px)|Fade(px)|dimesions(px)|color|

All of them with the color exception are in **px**.
 And also follow the table order.
- spread and blur are optional. Color is with rgba()
- We can "stack" multiple shadow boxes with a comma. 

#### Hover option
Within the style tag we can use the on hover.
```html 
element : hover{}
```

# POSITIONS
- `Relative position`
Move the element Relative to its current position. And we can move the element with the positions.
 * left, right, top, bottom with percentages, ems or pixels.
The elements around it still behave as if that item were in its default position. Doesn't remove it from the normal flow.

<img src="https://miro.medium.com/max/910/1*3N2ousp3yth9ovHA8TpDZw.png">

- `Absolute Positions`
Lock the element in place relative to its parent, removes the element to the normal flow. Sorrounding elements ignore it.
 -Position an element based on its closest positioned ancestor position.

<img src="https://miro.medium.com/max/686/1*XDqGjAEa_sNL1OlPQhEb7A.png">

- `Static position`

<img src="https://miro.medium.com/max/858/1*iVt-tUfGKHZyEkspuu7LlQ.png">

- `Fixed position` it's like absolute, the elements don't realize it is there, but the difference between absolute and fixed, is that fixed won't move wont scrolling. We can position it as well with right/top/bottom/left.

- `Float attribute` it's not a complete 'position' but it allow you to place elements to the left or right position removing it from the normal flow, eventhough they are not removed from the flow. It could be combined with inline elements.

* If elements are overlaped we can select their stack position with the `z-index:` property.

## Center a BLOCK element

We can do it with `margin: auto` property.

#### Color transition

With `linear-gradien(gradient-direction(deg), color1, color2, color3 ....)`
- Or also with `repeating-linear-gradient( direction, color stop, color stop, color stop ... )`
When the stops(in px) are the same, we generate stripes, if the stops are not the same we generate colors blend.

#### Background image
We can add an url image with `background: url( url-to-image )`

#### Change the element with the transform property
```css
transform: scale( x-times-to-scale )
transform: skewX( degrees )
transform: rotate( degrees )
```
#### before and after pseudo elements
They required the `content=""` which is used to add text or images while `::before` and `::after` are used to create shapes.
```css
.heart::after {
    background-color: blue;
    content: "";
    border-radius: 25%;
    position: absolute;
    width: 50px;
    height: 50px;
    top: 0px;
    left: 25px;
  }
  .heart::before {
    content: "";
    background-color: pink;
    border-radius: 50%;
    position: absolute;
    width: 50px;
    height: 50px;
    top: -25px;
    left: 0px;
  }
```
