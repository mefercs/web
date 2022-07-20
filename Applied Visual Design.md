# Applied Visual Design

- Opacity: 0 - 1

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


Last stuff
Lock an Element to the Browser Window with Fixed Positioning
